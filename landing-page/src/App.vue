<template>
  <main>
    <NavigationComponent />
    <section><MainText /></section>
  </main>
</template>

<script>
import NavigationComponent from "./components/Navigation/NavigationComponent.vue";
import MainText from "./components/Text/MainText.vue";

export default {
  name: "App",
  components: { NavigationComponent, MainText },
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
