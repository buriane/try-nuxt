<script lang="ts" setup>
import { useRouter } from 'vue-router';

const router = useRouter();

const navigateToHome = () => {
    router.push('/');
};
</script>

<template>
    <button @click="navigateToHome">
        Ini button
    </button>
</template>