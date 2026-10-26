<script setup>
import ProjectArticle from './ProjectArticle.vue';


</script>

<template>
    <section class="flex flex-col items-center gap-8 m-8 w-full max-w-6xl mx-auto">
        <h2 class="text-3xl font-bold text-center">
            <span class="font-bold text-gradient">Proyectos</span> realizados
        </h2>

        <!-- Renderizamos usando v-for para evitar duplicar código -->
        <div class="flex flex-col gap-8 w-full">
            <ProjectArticle />
        </div>
    </section>
</template>