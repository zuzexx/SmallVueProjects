<template>
  <section>
    <LeftChatter text="Hey! How can I help ypu today?" />
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
section {
  width: 80vw;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  margin-top: -0.25rem;
}
</style>
