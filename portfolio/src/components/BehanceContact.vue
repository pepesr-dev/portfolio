<script setup>
defineProps({
    link: String
})
</script>

<template>

    <a class="hover:text-accent-green p-2 border  rounded-xl border-glow inline-flex gap-1" :href="link"
        target="_blank">
        <img src="../assets/icons/icons/behance-black.svg" alt="Behance" class="block dark:hidden" />
        <img src="../assets/icons/icons/behance-white.svg" alt="Behance" class="hidden dark:block" />
        <span class=" font-bold">Guía de diseño</span>
    </a>

</template>