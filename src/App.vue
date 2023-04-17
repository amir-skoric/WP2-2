<script setup>
import Header from './components/MainHeader.vue';
import Section from './components/ContentSection.vue'
import Footer from './components/MainFooter.vue'

</script>

<template>
  <Header />
  <Section :textContent="'Hello this is content on the frontpage'" />
  <Footer />
</template>

