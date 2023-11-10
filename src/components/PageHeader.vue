<script setup lang="ts">
import { ref } from 'vue';
let display = ref(true);

function toggleDisplay():void {
  console.log("hi")
  display.value = !display.value;
  console.log(display);
}
</script>

<template>
  <div class="navbar">
      <span class="navbar-brand mb-0 h1">PWF</span>
      <button @click="toggleDisplay" class="navbar-toggler">
      <span class="navbar-toggler-icon"></span>
    </button>
  </div>
  <div class="row navbar-nav" v-if="display">
      <router-link class="nav-item nav-link" to="/">Home</router-link>
      <router-link class="nav-item nav-link" to="/About">About</router-link>
      <a class="nav-item nav-link" href="https://www.kickstarter.com">KickStarter</a>
    </div>
</template>

<style scoped>
h1 {
  text-align: center;
}
span {
  color: gold;
}
.nav-item{
  color: gold;
}
</style>
