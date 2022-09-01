<template>
  <section class="hero is-fullheight has-background-black">
    <div class="hero-body">
      <div class="container">
        <figure class="image center">
          <img
            src="@/assets/bulma-logo.png"
            alt="bulma logo"
            style="max-width: 512px"
          />
        </figure>
      </div>
    </div>
  </section>
</template>
<script>
export default {
  name: "TopComponent",
};
</script>
<style scoped>
.center {
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>
