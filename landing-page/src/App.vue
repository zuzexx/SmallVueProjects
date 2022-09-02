<template>
  <main>
    <NavigationComponent />
    <section><MainText /><MainChatComponent /></section>
  </main>
</template>

<script>
import NavigationComponent from "./components/Navigation/NavigationComponent.vue";
import MainText from "./components/Text/MainText.vue";
import MainChatComponent from "./components/Chat/MainChatComponent.vue";

export default {
  name: "App",
  components: { NavigationComponent, MainText, MainChatComponent },
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
  overflow: auto;
  font-family: var(--text-main);
}
</style>
