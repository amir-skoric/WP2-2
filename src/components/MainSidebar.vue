<script setup>
import { defineProps } from 'vue';

defineProps({
    textSidebar: {
        type: String
    }
})
</script>

<template>
    <aside>
        <p> {{ textSidebar }} </p>
    </aside>
</template>

<style >
aside {
    background: lightgray;
    position: sticky;
    width: 40%;
    text-align: center;
}
</style>