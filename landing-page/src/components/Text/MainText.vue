<template>
  <section class="text-section">
    <h1>Chatty chat</h1>
    <p>
      With Chatty chat software you can qualify leads faster. automatically book
      meetings for your sales team, and connect your costumers with the right
      business solutions more efficiently.
    </p>
    <Input />
  </section>
</template>
<script>
import Input from "./Input.vue";
export default {
  name: "MainText",
  components: { Input },
};
</script>
<style scoped>
.text-section {
  display: flex;
  flex-direction: column;
  width: 100vw;
  margin-top: 1rem;
  align-items: center;
}
p {
  width: 80vw;
  text-align: center;
  font-weight: 300;
  margin-top: -1rem;
}
h1 {
  font-weight: 700;
  font-size: 2.5rem;
}
@media only screen and (min-width: 1000px) {
  p {
    width: 40vw;
    text-align: left;
  }
  .text-section {
    width: 40vw;
    align-items: flex-start;
    margin-top: -7rem;
  }
  h1 {
    text-align: left;
  }
}
@media only screen and (min-width: 1400px) {
  p {
    font-weight: 400;
    font-size: 1.3rem;
    width: 730px;
  }
  h1 {
    font-weight: 900;
    font-size: 4rem;
    margin-top: -7rem;
  }
  .text-section {
    padding: 2rem;
  }
}
</style>
