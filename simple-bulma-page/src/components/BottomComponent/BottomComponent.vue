<template>
  <section>
    <div class="container">
      <div class="columns is-multiline">
        <div v-for="text in texts" :key="text" class="column is-one-third">
          <article class="media notification has-background-white">
            <figure class="media-left">
              <img :src="text.image" alt="icon" />
            </figure>
            <div class="media-content">
              <div class="content">
                <h1 class="title is-size-5">{{ text.title }}</h1>
                <p class="subtitle is-size-6">
                  {{ text.paragraph }}
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
  name: "BottomComponent",
  data() {
    return {
      texts: [
        {
          title: "Columns",
          paragraph: "The power of flexbox in a simple interface",
          image: "https://cdn-icons-png.flaticon.com/512/2147/2147718.png",
        },
        {
          title: "Form",
          paragraph:
            "The indispensable form controls, designed for maximum clarity",
          image: "https://cdn-icons-png.flaticon.com/512/2147/2147794.png",
        },
        {
          title: "Components",
          paragraph:
            "Advanced multi-part components with lots of possibilities",
          image: "https://cdn-icons-png.flaticon.com/512/2147/2147767.png",
        },
        {
          title: "Modifiers",
          paragraph: "An easy-to-read naming system designed for humans",
          image: "https://cdn-icons-png.flaticon.com/512/2147/2147779.png",
        },
        {
          title: "Layout",
          paragraph:
            "Design the structure of your webpage with these CSS classes",
          image: "https://cdn-icons-png.flaticon.com/512/2147/2147771.png",
        },
        {
          title: "Elements",
          paragraph:
            "Essential interface elements that only require a single CSS class",
          image: "https://cdn-icons-png.flaticon.com/512/2147/2147719.png",
        },
      ],
    };
  },
};
</script>
<style scoped>
img {
  width: 20px;
}
</style>
