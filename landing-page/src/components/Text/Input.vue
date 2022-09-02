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
@media only screen and (min-width: 1000px) {
  form {
    width: 40vw;
    justify-content: flex-start;
  }
  input {
    width: 30vw;
  }
}
@media only screen and (min-width: 1200px) {
  input {
    padding: 20px;
    max-width: 550px;
  }
  form {
    max-width: 700px;
  }
}
</style>
