<script setup lang="ts">
    const route = useRoute();
    const text = route.params.text as string;
</script>

<template>
    The text is: {{ text }}
</template>