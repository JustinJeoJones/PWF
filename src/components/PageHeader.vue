<script setup lang="ts">
import { ref } from "vue";
let display = ref(false);

function toggleDisplay(): void {
  display.value = !display.value;
}
</script>

<template>
  <div class="nav-bg sticky-top">
    <div
      class="navbar navbar-dark"
      @click="toggleDisplay"
    >
    
      <span class="navbar-brand m-0">
        <router-link class="nav-item nav-link" to="/">PWF</router-link>
      </span>
      <button class="navbar-toggler ">
        <span class="navbar-toggler-icon"></span>
      </button>
    </div>
    <div class="row navbar-nav" v-if="display">
      <router-link class="nav-item nav-link" to="/">Home</router-link>
      <router-link class="nav-item nav-link" to="/About">About</router-link>
      <a
        class="nav-item nav-link"
        target="_blank"
        href="https://docs.google.com/document/d/1RKKp6Gz9UnBn8Rxe7ItwjK645e_UHpY645iOJm72lDo/preview"
        >Rules</a
      >
      <a class="nav-item nav-link" href="https://www.kickstarter.com/projects/pwf/pro-wrestling-factions-pwf"
        >KickStarter</a
      >
    </div>
  </div>
</template>

<style scoped>
h1 {
  text-align: center;
}
span {
  color: gold;
}
.nav-item {
  color: gold;
}
.nav-bg {
  border-bottom: black 1px solid;
  background-color: rgb(53, 51, 51);
}
</style>
