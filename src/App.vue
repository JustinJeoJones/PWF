<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
import PageHeader from './components/PageHeader.vue'
import 'bootstrap/dist/css/bootstrap.min.css'
import 'bootstrap/js/dist/modal'
</script>

<template>
  <PageHeader />
  <div class="container">
    <RouterView />
  </div>
  
  
</template>

<style scoped>

</style>
