<template>
  <section class="section has-background-light">
    <div class="container">
      <div class="columns">
        <div class="column">
          <article class="media notification is-primary">
            <figure class="media-left">
              <img src="@/assets/code-language.png" alt="icon" />
            </figure>
            <div class="media-content">
              <div class="content">
                <h1 class="title is-size-5">Bulma?</h1>
                <p class="is-size-6">
                  Bulma is a modern CSS framework from @jgthms, based on
                  flexbox. Using Bulma, we can describe our website's design
                  using just classes.
                </p>
              </div>
            </div>
          </article>
        </div>
        <div class="column">
          <article class="media notification is-info">
            <figure class="media-left">
              <img src="@/assets/code.png" alt="icon" />
            </figure>
            <div class="media-content">
              <div class="content">
                <h1 class="title is-size-5">...Flexbox?</h1>
                <p class="is-size-6">
                  Flexbox is a CSS spec that makes sectioning and aligning more
                  natural. We do not need to know flexbox but it's how Bulma
                  works behind-the-scenes.
                </p>
              </div>
            </div>
          </article>
        </div>
        <div class="column">
          <article class="media notification is-warning">
            <figure class="media-left">
              <img src="@/assets/coffee-mug.png" alt="icon" />
            </figure>
            <div class="media-content">
              <div class="content">
                <h1 class="title is-size-5">...Classes?</h1>
                <p class="is-size-6">
                  Instead of writing our CSS per-element, we can use predefined
                  classes. With enough classes, we can describe our
                  websitedesign using semantics.
                </p>
              </div>
            </div>
          </article>
        </div>
      </div>
    </div>
  </section>
</template>
<script>
export default {
  name: "MiddleComponent",
};
</script>
<style scoped>
.margin {
  margin: 10px;
}
img {
  width: 27px;
  height: auto;
}
</style>
