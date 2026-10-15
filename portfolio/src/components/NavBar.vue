<script setup lang="ts">
import DarkMode from './DarkMode.vue';

</script>

<template>

    <header class="flex items-center justify-center gap-8 w-full p-4 shadow-md dark:shadow-none ">
        <!-- Menú de navegación centrado 🧭 -->
        <nav>
            <ul class="flex items-center gap-6">
                <li><a href="#">Inicio</a></li>
                <li><a href="#">Proyectos</a></li>
                <li><a href="#">Sobre mí</a></li>
            </ul>
        </nav>

        <!-- Conmutador de tema 🌙 -->
        <DarkMode />
    </header>
</template>