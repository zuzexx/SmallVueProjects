<template>
  <form>
    <input type="text" placeholder="Email Adress" />
    <Buttons text="I want a demo" class="primary but" />
  </form>
</template>
<script>
import Buttons from "../Reusable/Buttons.vue";

export default {
  name: "Input",
  components: { Buttons },
};
</script>
<style scoped>
input {
  padding: 15px;
  border: 1px solid var(--button-color);
  border-radius: 0.25rem;
  font-family: var(--text-main);
  color: var(--background-color);
  width: 40vw;
  outline: none;
  max-width: 500px;
}
form {
  width: 80vw;
  display: flex;
  flex-direction: row;
  justify-content: center;
}
.but {
  margin-left: -1rem;
}
</style>
