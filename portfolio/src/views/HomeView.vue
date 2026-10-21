<script setup>
import AboutMeSection from '@/components/AboutMeSection.vue';
import FooterCredits from '@/components/FooterCredits.vue';
import HomeHero from '@/components/HomeHero.vue';
import NavBar from '@/components/NavBar.vue';



</script>
<template>
    <div class="px-4 max-w-7xl w-full m-auto">

        <header>
            <div class="mt-12.5 w-full flex justify-center">
                <NavBar />
            </div>

            <HomeHero />


        </header>

        <main class="w-full">
            <AboutMeSection />
        </main>

    </div>
    <footer class="w-full text-center">
        <FooterCredits />
    </footer>
</template>