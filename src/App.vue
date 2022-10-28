<script>
import Header from "./components/Header.vue";
import Audio from "./components/Audio.vue";
export default {
  components: {
    Header,
    Audio,
  },
};
</script>

<template>
  <div id="app">
    <Audio />
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
