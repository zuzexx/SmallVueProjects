<template>
  <section class="chatting-section">
    <LeftChatter text="Hey! How can I help you today?" />
    <RightChatter text="I am interested in this chat." />
    <LeftChatter text="Great! You are in the right place!" />
    <RightChatter text="How can it help my company?" />
    <LeftChatter text="..." />
  </section>
</template>
<script>
import LeftChatter from "./LeftChatter.vue";
import RightChatter from "./RightChatter.vue";
export default {
  name: "Chatting",
  components: { LeftChatter, RightChatter },
};
</script>
<style scoped>
.chatting-section {
  width: 80vw;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  margin-top: -0.25rem;
}
@media only screen and (min-width: 1000px) {
  .chatting-section {
    width: 40vw;
  }
}
@media only screen and (min-width: 1200px) {
  .chatting-section {
    padding-top: 2rem;
    padding-bottom: 2rem;
    max-width: 550px;
  }
}
</style>
