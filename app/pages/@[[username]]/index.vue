<script setup lang="ts">
    const route = useRoute();
</script>

<template>
    <div>
        <p>{{ route.params }}</p>
        <h1>ini @ {{ route.params.username }} </h1>
    </div>
</template>