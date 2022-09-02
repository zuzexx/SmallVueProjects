<template>
  <section>
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
section {
  width: 100vw;
  display: flex;
  flex-direction: column;
  align-items: center;
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
</style>
