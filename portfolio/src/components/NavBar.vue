<script setup lang="ts">
import DarkMode from './DarkMode.vue';

</script>

<template>

    <header
        class="flex items-center justify-center gap-8 w-full pl-4 pr-4 p-1.5 shadow-md dark:shadow-none sm:w-max sm:border sm:rounded-full border-glow">
        <!-- Menú de navegación centrado 🧭 -->
        <nav>
            <ul class="flex items-center gap-6">
                <li><a class="hover:text-accent-green font-bold" href="#">Inicio</a></li>
                <li><a class="hover:text-accent-green font-bold" href="#">Proyectos</a></li>
                <li><a class="hover:text-accent-green font-bold" href="#">Sobre mí</a></li>
            </ul>
        </nav>

        <!-- Conmutador de tema 🌙 -->
        <DarkMode />
    </header>
</template>