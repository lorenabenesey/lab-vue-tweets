<template>
<span className="name">{{ name }}</span>
</template>



<script setup>
import { ref } from 'vue';
const props = defineProps(["name"]);
</script>



<style scoped>
</style>
