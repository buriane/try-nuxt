<script lang="ts" setup>
useSeoMeta({
    title: 'Netflix Page',
    description: 'Welcome to the Netflix page of our Nuxt application.',
});

definePageMeta({
    layout: 'false',
});
</script>

<template>
    <NuxtLayout name="dashboard">
    <div>
        <p>Parent Netflix</p>
        <NuxtPage />
    </div>
    </NuxtLayout>
</template>