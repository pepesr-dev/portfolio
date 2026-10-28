<script setup>
import AboutMeSection from '@/components/AboutMeSection.vue';
import FooterCredits from '@/components/FooterCredits.vue';
import HomeHero from '@/components/HomeHero.vue';
import NavBar from '@/components/NavBar.vue';
import ProyectsSection from '@/components/ProjectsSection.vue';



</script>
<template>
    <div class="w-full ">
        <div class="pl-2 pr-2 max-w-300 w-full m-auto">


            <header class="pt-12.5 w-full flex justify-center ">
                <NavBar />
            </header>

            <main class="w-full pl-2 pr-2 ">
                <HomeHero />
                <ProyectsSection />
                <AboutMeSection />
            </main>

        </div>
        <footer class="w-full text-center">
            <FooterCredits />
        </footer>
    </div>
</template>