<script lang="ts" setup>
useSeoMeta({
    title: 'Home Page',
    description: 'Welcome to the home page of our Nuxt application.',
});

const router = useRouter();

const navigateToNetflix = () => {
    // navigateTo({
    //     path: '/netflix',
    // });
    router.push('/netflix');
};
</script>

<template>
    <div>
        <h1>Welcome to the Home Page</h1>
        <p>This is the content of the home page.</p>
        <div>
            <NuxtLink to="/netflix">Netflix </NuxtLink>
            <button @click="navigateToNetflix">Go to Netflix</button>
            <!-- <NuxtLink to="/about">About </NuxtLink>
            <NuxtLink to="/contact">Contact </NuxtLink> -->
        </div>
    </div>
</template>