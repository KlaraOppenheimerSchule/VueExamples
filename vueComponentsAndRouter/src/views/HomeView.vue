<script setup>
import { RouterLink, RouterView } from 'vue-router'
import Footer from '../components/Footer.vue'
</script>

<template>
  <RouterLink to="/">Home</RouterLink>
  <RouterLink to="/about">About</RouterLink>
  <h1> Home View</h1>
  <p> Central information home view </p>
  <Footer />
</template>

