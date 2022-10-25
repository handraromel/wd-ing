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
#app {
  font-family: "tss";
  color: #7c6a5e;
}
</style>
