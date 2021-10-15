<template>
  <main>
    <Hero />
    <FirstDrive />
    <Courses />
  </main>
</template>

<script>
import Hero from "./Hero.vue";
import FirstDrive from "./First-Drive.vue";
import Courses from "./Courses.vue";
export default {
  name: "Main",
  components: {
    Hero,
    FirstDrive,
    Courses,
  },
};
</script>

<style lang="scss" scoped>
@import "../assets/style/variables.scss";
</style>