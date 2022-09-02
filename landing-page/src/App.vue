<template>
  <main>
    <NavigationComponent />
    <section class="main-section"><MainText /><MainChatComponent /></section>
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
  overflow-y: auto;
  overflow-x: hidden;
  font-family: var(--text-main);
  display: flex;
  justify-content: center;
  align-items: center;
}
@media only screen and (min-width: 1000px) {
  .main-section {
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    width: 100vw;
    padding: 2rem;
  }
}
</style>
