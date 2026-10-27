<script setup>
import BehanceContact from './BehanceContact.vue';
import DownloadCV from './DownloadCV.vue';
import GitHubContact from './GitHubContact.vue';
import LinkedInContact from './LinkedInContact.vue';
import MailContact from './MailContact.vue';
import WorkStatus from './WorkStatus.vue';

</script>
<template>

    <section class="mt-15 p-8 flex flex-col items-center text-center justify-center w-full mx-auto gap-4">
        <figure>
            <img class=" min-w-40 min-h-40 object-cover rounded-full" src="../assets/icons/jose/jose-profileImg.png"
                alt="jose">
        </figure>
        <WorkStatus />

        <div class="p-8 text-center">
            <h1 id="home" class="text-display text-gradient">José Serrano</h1>

            <h3><span class="  font-bold text-gradient">Desarrollador Web Full-Stack.</span> Vivo en Jerez de la
                frontera, Cádiz.</h3>

        </div>
        <div class="p-8 flex gap-2 flex-wrap justify-center">
            <!--Mail-->
            <MailContact />
            <LinkedInContact />
            <DownloadCV />
            <GitHubContact />
            <BehanceContact link="https://www.behance.net/pepesr" />


        </div>
    </section>



</template>