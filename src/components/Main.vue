<template>
  <main>
    <Hero />
    <FirstDrive />
  </main>
</template>

<script>
import Hero from "./Hero.vue";
import FirstDrive from "./First-Drive.vue";
export default {
  name: "Main",
  components: {
    Hero,
    FirstDrive,
  },
};
</script>

<style lang="scss" scoped>
@import "../assets/style/variables.scss";
</style>