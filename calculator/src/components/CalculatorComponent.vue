<template>
  <main>
    <section>
      <p>this is calculator</p>
    </section>
  </main>
</template>
<script>
export default {
  name: "CalculatorComponent",
};
</script>
<style scoped>
main {
  width: 100vw;
  height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}
section {
  border: 2px solid red;
  width: 60vw;
  min-width: 300px;
  max-width: 500px;
  height: 500px;
}
</style>
