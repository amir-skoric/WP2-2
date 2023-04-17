<script setup>
import { defineProps } from 'vue';
import Sidebar from './MainSidebar.vue'

defineProps({
    textContent: {
        type: String
    }
})
</script>

<template>
    <div class="container">
        <section>
            <h2>{{ textContent }}</h2>
            <p>Test</p>
        </section>
        <Sidebar :textSidebar="'Aside text :)'" />
    </div>
</template>

<style scoped>
.container {
    height: 85vh;
    display: flex;
    flex-direction: row;
    margin-bottom: 50px;
}
section {
    background: white;
    padding: 20px;
    width: 100%;
}
</style>