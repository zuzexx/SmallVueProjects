<template>
  <section class="main-chat-section">
    <div class="background"><Chatting /></div>
  </section>
</template>
<script>
import Chatting from "./Chatting.vue";

export default {
  name: "MainChatComponent",
  components: { Chatting },
};
</script>
<style scoped>
.main-chat-section {
  width: 100vw;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  margin-top: 2rem;
  justify-content: center;
}
.background {
  background-color: var(--svg-one);
  border-radius: 0.25rem;
  width: 80vw;
  height: auto;
  padding: 0.5rem;
}
@media only screen and (min-width: 1000px) {
  .main-chat-section {
    width: 50vw;
  }
  .background {
    width: 40vw;
  }
}
@media only screen and (min-width: 1200px) {
  .main-chat-section {
    max-width: 550px;
    padding: 2rem;
  }
  .background {
    max-width: 550px;
  }
}
</style>
