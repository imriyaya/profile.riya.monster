<script setup lang="ts">
import Button from "../components/Button.vue"
</script>

<template>
  <main class="background">
    <div class="wrapper">
      <img src="/icon.jpg" alt="icon" class="icon">
      <h1>Welcome to <span>riya</span>'s link site!</h1>
      <h2>See what I am up to~</h2>
      <Button path="https://instagram.com/imriyaya">Instagram</Button>
      <Button path="https://twitter.com/imriyaya">Twitter</Button>
      <Button path="https://www.youtube.com/@t.z">Youtube</Button>
      <Button path="https://discord.com/invite/NJkb2TdR2x">Discord</Button>
      <Button path="https://github.com/imriyaya">GitHub</Button>
      <Button path="https://soundcloud.com/imriya">SoundCloud</Button>
    </div>
  </main>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Pacifico&display=swap');

* {
  font-family: "Pacifico", cursive;
  font-weight: 400;
  font-style: normal;
  color: white;
  text-shadow: 5px 5px 5px rgba(0, 0, 0, 1);
  user-select: none;
}

.background {
  min-height: 100vh;
  width: 100vw;
  background-image: url("/wallpaper.jpg");
  background-repeat: no-repeat;
  background-size: cover;
}

.wrapper {
  min-height: 100vh;
  width: 600px;
  margin: 0 auto;
  text-align: center;
  background-color: rgba(0, 0, 0, 30%);
  box-shadow: 0 0 50px rgba(0, 0, 0, 50%);
  backdrop-filter: blur(5px);
}

.icon {
  width: 200px;
  height: 200px;
  border-radius: 100%;
  margin-top: 5em;
  box-shadow: 0 0 30px rgba(0, 0, 0, 100%);
}

@media screen and (max-width: 1000px) {
  .wrapper {
    width: 90%;
  }
}
</style>