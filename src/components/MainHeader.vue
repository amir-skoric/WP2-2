<script setup>
import { ref } from 'vue';

const links = ref(['Page 1', 'Page 2', 'Page 3', 'Page 4'])
</script>

<template>
    <header>
        <h2><a href="#">Website</a></h2>
        <ul>
            <li v-for="link, key in links" :key="key"><a href="#">{{ link }}</a></li>
        </ul>
    </header>
</template>

<style>
header {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
    background: lightblue;
    padding: 20px;
}

header h2>a {
    text-decoration: none;
}

header ul {
    display: flex;
    list-style-type: none;
}

header li {
    padding: 20px
}
</style>