<template>
  <div class="container under-line-thin mt-2">
    <nav class="navbar is-transparent">
      <div class="navbar-brand">
        <a class="navbar-item" href="http://www.c14.pl">
          <img class="nav-img" src="/img/logo.jpg" alt="LOGO" />
        </a>
        <div class= "lab-cl">
          <span class="lab-up">{{ lab_label }}</span>
          <span class="lab-down">{{ small_label }}</span>
        </div>
        <div class="navbar-item lang-ver" @click="clickToggleLang()">{{ jezyk }}</div>
      </div>

      <div id="navbarExampleTransparentExample" class="navbar-menu"></div>
    </nav>
  </div>
</template>

<script>
export default {
  emits: ["toggle-lang"],
  data() {
    return {
      jezyk: "english version",
      lab_label: "LABORATORIUM",
      small_label: "DATOWAŃ BEZWZGLĘDNYCH",
    };
  },
  methods: {
    clickToggleLang() {
      if (this.jezyk === "english version") {
        this.jezyk = "polish version";
        this.lab_label = "LABORATORY";
        this.small_label = "OF ABSOLUTE DATING";
      } else {
        this.jezyk = "english version";
        (this.lab_label = "LABORATORIUM"),
          (this.small_label = "DATOWAŃ BEZWZGLĘDNYCH");
      }
      this.$emit("toggle-lang");
    },
  },
};
</script>

<style scoped>
.navbar-brand {
  flex-wrap: wrap-reverse;
}
.lang-ver {
  display: flex;
  position: relative;
  flex-direction: column;
  justify-content: flex-end;
  align-items: flex-end;
  height: 100%;
  font-size: 10pt;
  cursor: pointer;
}

.lab-cl {
  position: relative;
  width: 280px;
  min-width: 280px;
  font-family: "Montserrat", "Helvetica Neue", Helvetica, Arial, sans-serif;
  font-weight: 700;
}

.lab-up {
  position: absolute;
  top: 33px;
  font-size: 28px;
  min-width: 280px;
}

.lab-down {
  position: absolute;
  min-width: 280px;
  top: 60px;
  left: 3px;
  font-size: 15px;
}

.lab-desc {
  display: block;
  font-size: 15pt;
  text-align: justify;
  padding: 30px;
}

.under-line-thin {
  border-bottom: 1px solid rgb(230, 230, 230);
}
.under-line-thin::after {
  content: "";
  width: 480px;
  display: block;
  border-bottom: 1px solid #007dc6;
  transform: translateY(1px);
  z-index: 11200;
}
</style>
