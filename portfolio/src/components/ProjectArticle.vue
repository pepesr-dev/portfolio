<script setup>
import BehanceContact from './BehanceContact.vue';
import CodeButtom from './CodeButtom.vue';
import PreviewButton from './PreviewButton.vue';
import taskListImg from '../assets/img/task-list.png';
import iteraAppImg from '../assets/img/iteraApp.jpg';

</script>

<template>
    <!-- Contenedor principal con diseño responsivo e inversión de orden -->
    <article class="flex flex-col md:flex-row items-center gap-8 p-6 md:p-8">


        <figure>
            <img class="  border-glow  rounded-2xl min-w-120 min-h-60" :src="iteraAppImg" alt="itera img">

        </figure>

        <div class="w-full md:w-1/2 flex flex-col gap-4 md:gap-10 text-left">

            <div>
                <h3 class="font-bold dark:text-dark">Itera</h3>
                <h1 class="  font-bold dark:text-gradient">
                    Buscador visual y red social
                </h1>
            </div>
            <div>

                <div class="flex flex-wrap gap-2 dark:text-dark mb-2">

                    <p class="p-1 pr-2 pl-2 font-bold  bg-accent-green text-white rounded-full">#PHP</p>
                    <p class="p-1 pr-2 pl-2 font-bold  bg-accent-green text-white rounded-full">#Vue.js</p>
                    <p class="p-1 pr-2 pl-2 font-bold  bg-accent-green text-white rounded-full">#Laravel</p>

                </div>

                <p class="dark-text-dark">
                    Aplicación web full-stack que replica la lógica y el diseño de Pinterest.
                    Presenta la colección de imágenes publicadas por los usuarios en formato mampostería y permite la
                    gestión de las mismas.
                </p>
                <div class=" pt-2 flex gap-2 flex-wrap ">
                    <PreviewButton />
                    <CodeButtom />
                    <BehanceContact
                        link="https://www.behance.net/gallery/256949487/Portfolio-web-Guia-de-estilos/modules/1500391247" />
                </div>

            </div>

        </div>

    </article>

    <!--REVERSE PROYECT-->
    <article class="flex flex-col md:flex-row items-center gap-8 p-6 md:p-8">


        <figure>
            <img class="  border-glow  rounded-2xl min-w-120 min-h-60" :src="taskListImg" alt="taskList img">

        </figure>

        <div class="w-full md:w-1/2 flex flex-col gap-4 md:gap-10 text-left">

            <div>
                <h3 class="font-bold dark:text-dark">TaskList</h3>
                <h1 class="  font-bold dark:text-gradient">
                    Gestor web de tareas
                </h1>
            </div>
            <div>

                <div class="flex flex-wrap gap-2 dark:text-dark mb-2">


                    <p class="p-1 pr-2 pl-2 font-bold  bg-accent-green text-white rounded-full">#HTML</p>
                    <p class="p-1 pr-2 pl-2 font-bold  bg-accent-green text-white rounded-full">#CSS</p>
                    <p class="p-1 pr-2 pl-2 font-bold  bg-accent-green text-white rounded-full">#SQL</p>
                    <p class="p-1 pr-2 pl-2 font-bold  bg-accent-green text-white rounded-full">#MySQL</p>
                    <p class="p-1 pr-2 pl-2 font-bold  bg-accent-green text-white rounded-full">#PHP</p>

                </div>

                <p class="dark-text-dark">
                    App web desarrollada con PHP nativo y conectada a una base de datos relacional MySql. Este proyecto
                    cuenta con una interfaz de usuario con diseño 100% propio.
                </p>
                <div class=" pt-2 flex gap-2 flex-wrap ">
                    <PreviewButton />
                    <CodeButtom />
                    <BehanceContact
                        link="https://www.behance.net/gallery/256949487/Portfolio-web-Guia-de-estilos/modules/1500391247" />
                </div>

            </div>

        </div>

    </article>
</template>