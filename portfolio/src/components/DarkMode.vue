<script setup>
import { ref, onMounted } from 'vue'

// Oscuro 🌙
import moonDark from '../assets/icons/darkMode/darkModeIcon-moon-dark.svg'
import moonGreen from '../assets/icons/darkMode/darkModeIcon-moon-green.svg'
import moonGrey from '../assets/icons/darkMode/darkModeIcon-moon-grey.svg'

// Claro ☀️
import sunDark from '../assets/icons/darkMode/darkModeIcon-sun-drak.svg'
import sunGreen from '../assets/icons/darkMode/darkModeIcon-sun-green.svg'
import sunGrey from '../assets/icons/darkMode/darkModeIcon-sun-grey.svg'

// Sistema 🖥️
import systemDark from '../assets/icons/darkMode/darkModeIcon-system-dark.svg'
import systemGreen from '../assets/icons/darkMode/darkModeIcon-system-green.svg'
import systemGrey from '../assets/icons/darkMode/darkModeIcon-system-grey.svg'

// Estado del modo seleccionado ('light' | 'dark' | 'system')
const currentMode = ref('system')
// Estado de si el fondo actual de la app es oscuro
const isAppDark = ref(false)

const setTheme = (mode) => {
    currentMode.value = mode
    localStorage.setItem('theme', mode)

    const prefersDark = window.matchMedia('(prefers-color-scheme: dark)').matches

    if (mode === 'dark' || (mode === 'system' && prefersDark)) {
        document.documentElement.classList.add('dark')
        isAppDark.value = true
    } else {
        document.documentElement.classList.remove('dark')
        isAppDark.value = false
    }
}

onMounted(() => {
    const savedTheme = localStorage.getItem('theme') || 'system'
    setTheme(savedTheme)
})
</script>

<template>
    <div
        class="inline-flex items-center gap-2 p-1 rounded-full border-2 border-transparent bg-origin-border [background-clip:padding-box,border-box] bg-[linear-gradient(var(--color-bg-light),var(--color-bg-light)),linear-gradient(to_right,var(--color-accent-green),var(--color-accent-blue))] dark:bg-[linear-gradient(var(--color-bg-dark),var(--color-bg-dark)),linear-gradient(to_right,var(--color-accent-green),var(--color-accent-blue))]">
        <!-- Botón 1: Modo Oscuro 🌙 -->
        <button type="button" @click="setTheme('dark')">
            <img :src="currentMode === 'dark' ? moonGreen : (isAppDark ? moonDark : moonGrey)" alt="Modo Oscuro" />
        </button>

        <!-- Botón 2: Modo Claro ☀️ -->
        <button type="button" @click="setTheme('light')">
            <img :src="currentMode === 'light' ? sunGreen : (isAppDark ? sunDark : sunGrey)" alt="Modo Claro" />
        </button>

        <!-- Botón 3: Modo Sistema 🖥️ -->
        <button type="button" @click="setTheme('system')">
            <img :src="currentMode === 'system' ? systemGreen : (isAppDark ? systemDark : systemGrey)"
                alt="Modo Sistema" />
        </button>
    </div>
</template>