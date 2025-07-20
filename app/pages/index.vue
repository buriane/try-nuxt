<script lang="ts" setup>
useSeoMeta({
    title: 'Home Page',
    description: 'Welcome to the home page of our Nuxt application.',
});

definePageMeta({
    layout: 'dashboard',
});

const router = useRouter();

const navigateToNetflix = () => {
    // navigateTo({
    //     path: '/netflix',
    // });
    router.push('/netflix');
};

const changeLayoutToDefault = () => {
    setPageLayout('default');
};
</script>

<template>
    <div>
        <img src="~/assets/logo/logo-green-white.png" alt="logo">
        <h1>Welcome to the Home Page</h1>
        <p>This is the content of the home page.</p>
        <div>
            <NuxtLink to="/netflix">Netflix </NuxtLink>
            <button class="btn btn-primary" @click="navigateToNetflix">Button Bootstrap</button>
            <button @click="navigateToNetflix">Go to Netflix</button>
            <button @click="changeLayoutToDefault">Change Layout to Default</button>
            <!-- <NuxtLink to="/about">About </NuxtLink>
            <NuxtLink to="/contact">Contact </NuxtLink> -->
        </div>
    </div>
</template>

<style scoped>
* {
    background: green;
}
</style>