<template>
  <div id="app">
    <Header />
    <ComicsList />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import ComicsList from "./components/ComicsList.vue";

export default {
  name: "App",
  components: {
    Header, ComicsList,
  }
};
</script>

<style lang="scss">
@import "./style/general.scss";
@import "./style/variables.scss";
</style>
