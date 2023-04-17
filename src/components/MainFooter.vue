<script setup>
import { ref } from 'vue';
const footerText = ref('Website created in Vue 3')
</script>

<template>
    <footer>
        <h3>{{ footerText }}</h3>
    </footer>
</template>

<style>
footer {
    background: black;
    padding: 20px;
    position: fixed;
    width: 100%;
    bottom: 0;
}

footer h3 {
    color: white;
}
</style>