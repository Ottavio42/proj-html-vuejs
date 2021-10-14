<template>
  <div id="app">
    <Header :headerNav="headerNav" />
    <Main />
    <Footer :footerNav="footerNav" />
  </div>
</template>

<script>
import "@fortawesome/fontawesome-free/js/all.js";
import Header from './components/Header.vue';
import Main from './components/Main.vue';
import Footer from './components/Footer.vue';


export default {
  name: 'App',
  components: {
    Header,
    Footer,
    Main,
  },
  data() {
    return {
      headerNav: ["HOME", "ABOUT", "PRICES", "COURSES", "BLOG", "BOOK NOW"],
      footerNav: {
        information: [
          {
            word: "123456 North Main Street, New York, NY 555555",
            fawesome: "fas fa-home",
          },
          {
            word: "0.003.965.98",
            fawesome: "fas fa-phone",
          },
          {
            word: "info-yourdomain.com",
            fawesome: "fas fa-envelope",
          },
          {
            word: "theme-fusion.com",
            fawesome: "fas fa-link",
          }
        ],
        courses: ["Pass Plus", "Intensive Course", "Automatic", "Istructor Training"]

      }
    }
  }

}
</script>

<style lang="scss">
// Common
@import "./assets/style/common.scss";
// Variables
@import "./assets/style/variables.scss";
// Font
@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@100;300;400;500;700;800&display=swap');

</style>
