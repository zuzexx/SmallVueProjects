<template>
  <main><NavigationComponent /></main>
</template>

<script>
import NavigationComponent from "./components/Navigation/NavigationComponent.vue";

export default {
  name: "App",
  components: { NavigationComponent },
};
</script>
<style scoped>
@import "@/styles.css";
main {
  background-color: var(--background-color);
  color: var(--text-color);
  width: 100vw;
  height: 100vh;
  margin: -8px;
  overflow: hidden;
  font-family: var(--text-main);
}
</style>
