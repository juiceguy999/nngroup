<script setup>
import TheFooter from '@/components/TheFooter.vue';
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <div class="wrapper">
    <RouterView />
    
    <TheFooter />
  </div>

</template>

<style>

  html, body, #app {
    height: 100%;
  }

  .container {
    max-width: 1220px;
    margin: 0 auto;
    padding: 0 10px;
  }

  .wrapper {
    min-height: 100%;
    display: flex;
    flex-direction: column;
  }

  .main {
    flex-grow: 1;
  }
</style>
