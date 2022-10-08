<script>
import Header from "./components/Header.vue";
// import Navbar from "./components/Navbar.vue"
export default {
  components: {
    Header,
    // Navbar
  },
};
</script>

<template>
  <div id="app">
    <!-- <Navbar /> -->
    <Header />
    <main></main>
  </div>
</template>

<style scoped>
@font-face {
  font-family: "nunito";
  src: url(@/assets/fonts/nunito.ttf);
}
@font-face {
  font-family: "fajardo";
  src: url(@/assets/fonts/fajardo.ttf);
}

#app {
  font-family: "nunito";
  color: #7c6a5e;
  background: url(@/assets/img/header-bg.webp) center no-repeat;
  background-size: cover;
}
</style>
