<script setup lang="ts">
let Backers:string[] = [];
</script>

<template>
  <main>
    <h1>Pro Wrestling Factions</h1>
    <div class="row">
      <p>Try to manage the chaos of Pro Wrestling Factions</p>
    </div>
    <div class="row">
      <img
        class="col-12 col-md-6 offset-md-3"
        src="../assets/Gruntz-Boxart-MainFace.png"
      />
    </div>
    <div class="row">
      <p>Check out our Kickstarter video here!</p>
    </div>
    <div class="row">
      <video class="col-md-6 offset-md-3" controls ><source src="../assets/KickstarterVid.mp4"> </video>
    </div>
    <div>
      <p>Support us on <a href="https://www.kickstarter.com/projects/pwf/pro-wrestling-factions-pwf">KickStarter</a></p>
      <iframe src="https://www.kickstarter.com/projects/pwf/pro-wrestling-factions-pwf/widget/card.html?v=2" width="220" height="420" frameborder="0" scrolling="no"></iframe>
    </div>
    <div class="row"><h2>Build your roster!</h2></div>
    <div class="row">
      <p>
        Recruit your talent and work up to challenge Superstars!
      </p>
    </div>
    <div class="row align-items-end">
      <div class="col-6">
        <h3>Will you run a successful empire?</h3>
        <img height="150px" src="..\assets\Gruntz-Boxart-CardPile-Originals-01.png" />
      </div>
      <div class="col-6">
        <h3>Or will you be forced to retire?</h3>
        <img height="150px" src="..\assets\Gruntz-Boxart-CardPile-Originals-02.png" />
      </div>
    </div>
    <div class="row"><h2>Two ways to play!</h2></div>
    <div class="row">
      <p>
        Explore a brief narrative in the 3-month mode or immerse yourself in a comprehensive storyline by opting for the full-year experience. Every playthrough is different as randomized Events change the story!
      </p>
    </div>
    <div class="row" >
      <div class="col-6 offset-3"><img  src="..\assets\Gruntz-Boxart-CardPile-Originals-00.png" /></div>
      
    </div>
    <div class="row">
      <p>2-4 Players</p>
      <p>30 minutes - 1 hour to play</p>
      <p>Or as long as you'd like!</p>
      <p>Ages: 14+</p>
      <p>Contains small parts</p>
    </div>

    <div class="row"><h2>Special thanks to all of our Backers!</h2></div>
    <div class="row"><p>Last updated 11/16/2023</p></div>

    <p v-for="b in Backers">
      {{ b }}
    </p>
  </main>
</template>

<style scoped>
</style>
