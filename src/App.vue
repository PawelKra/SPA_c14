<template>
  <nav-bar @toggle-lang="changeShownLanguage()"></nav-bar>
  <main-page :lindex="lata"></main-page>
  <PageFooter />
</template>

<script>
import NavBar from "./components/NavBar.vue";
import MainPage from "./components/MainPage.vue";
import PageFooter from "./components/PageFooter.vue";
import { computed } from "@vue/runtime-core";

export default {
  name: "App",
  components: {
    NavBar,
    MainPage,
    PageFooter,
  },
  data() {
    return {
      pllanguage: true,
      lata: 1, // 1-polski, 0-eng
    };
  },
  provide: {
    pllanguage: computed(() => this.pllanguage),
  },
  methods: {
    changeShownLanguage() {
      this.pllanguage = !this.pllanguage;
      if (this.pllanguage) {
        this.lata = 1;
      } else {
        this.lata = 0;
      }
    },
  },
  // created() {
  //   var lang = (navigator.languages && navigator.languages[0]) || "";
  //   if (lang === "pl") {
  //     this.lata = 1;
  //   } else {
  //     this.lata = 0;
  //   }
  // },
};
</script>

<style>
#app {
  /* font-family: Avenir, Helvetica, Arial, sans-serif; */
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  min-width: 480px;
}
</style>
