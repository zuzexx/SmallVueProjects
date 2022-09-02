<template>
  <nav class="navigation">
    <div class="header-div"><h2>Chatty</h2></div>
    <div class="buttons">
      <Buttons text="get a demo" class="primary" /><Buttons
        text="sign in"
        class="secondary"
      />
    </div>
  </nav>
</template>
<script>
import Buttons from "../Reusable/Buttons.vue";
export default {
  name: "NavigationComponent",
  components: { Buttons },
};
</script>
<style scoped>
.navigation {
  width: 100vw;
  height: 4rem;
  font-size: 1rem;
}
.header-div {
  height: 2rem;
  display: flex;
  align-content: center;
  margin-left: 2rem;
}
h2 {
  justify-items: center;
}
.buttons {
  display: flex;
  flex-direction: row;
  margin-right: 2rem;
  justify-content: right;
  align-items: center;
  height: 10%;
}
.primary {
  background-color: var(--button-color);
  color: var(--background-color);
  border: 1px solid var(--button-color);
}
.primary:hover {
  cursor: pointer;
  background-color: var(--background-color);
  color: var(--button-color);
}
.secondary {
  background-color: var(--background-color);
  border: 1px solid var(--button-color);
  color: var(--button-color);
}
.secondary:hover {
  cursor: pointer;
  background-color: var(--button-color);
  color: var(--background-color);
}
@media only screen and (min-width: 1200px) {
  .primary:hover {
    border-width: 2px;
  }
  .secondary {
    border-width: 2px;
  }
  .primary {
    border-width: 2px;
  }
  h2 {
    font-size: 2rem;
  }
  .navigation {
    height: 6rem;
  }
  .buttons {
    height: 35%;
  }
}
</style>
