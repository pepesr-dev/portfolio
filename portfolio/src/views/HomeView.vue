<script setup>
import AboutMeSection from '@/components/AboutMeSection.vue';
import FooterCredits from '@/components/FooterCredits.vue';
import HomeHero from '@/components/HomeHero.vue';
import NavBar from '@/components/NavBar.vue';



</script>
<template>
    <div class=" max-w-7xl m-auto">
        <header>
            <div class=" mt-12.5 w-full flex justify-center">
                <NavBar />
            </div>

            <HomeHero />


        </header>

        <main>
            <AboutMeSection />

        </main>

    </div>
    <footer>

        <FooterCredits />
    </footer>
</template>