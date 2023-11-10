<script setup lang="ts">
const props = defineProps<{
  title?: string;
  image?: string;
}>();

console.log(props);
</script>

<template>
  <main>
    <div class="row">
        <p>{{ title }}</p>
    </div>
    <div class="row">
        <img :src="image" />
    </div>
  </main>
</template>

<style scoped>
h1 {
  text-align: center;
}
</style>
