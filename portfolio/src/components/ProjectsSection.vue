<script setup>
import ProjectArticle from './ProjectArticle.vue';


</script>

<template>
    <section class="pt-2 pb-2 flex flex-col items-center gap-4 w-full max-w-7xl mx-auto">
        <h2 id="proyects" class=" font-bold text-center">
            <span class="font-bold text-gradient">Proyectos</span> realizados
        </h2>


        <div class="flex flex-col gap-8 w-full">
            <ProjectArticle />
        </div>
    </section>
</template>