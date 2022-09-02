<template>
  <button>{{ text }}</button>
</template>
<script>
export default {
  name: "Buttons",
  props: {
    text: {
      type: String,
      required: true,
    },
  },
};
</script>
<style scoped>
@import "@/styles.css";
button {
  padding: 8px 17px;
  margin-left: 1rem;
  font-weight: 600;
  text-transform: uppercase;
  font-size: 0.7 rem;
  font-family: var(--text-main);
  border: none;
  border-radius: 0.25rem;
}
@media only screen and (min-width: 1200px) {
  button {
    padding: 12px 25px;
  }
}
</style>
