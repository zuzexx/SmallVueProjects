<template>
  <section class="right">
    <div class="bubble-right">
      <p>{{ text }}</p>
    </div>
    <div class="avatar-right">
      <svg
        viewBox="0 0 36 36"
        fill="none"
        role="img"
        xmlns="http://www.w3.org/2000/svg"
        width="80"
        height="80"
      >
        <title>Lucy Stone</title>
        <mask
          id="mask__beam"
          maskUnits="userSpaceOnUse"
          x="0"
          y="0"
          width="36"
          height="36"
        >
          <rect width="36" height="36" rx="72" fill="#FFFFFF"></rect>
        </mask>
        <g mask="url(#mask__beam)">
          <rect width="36" height="36" fill="#aaf8a0"></rect>
          <rect
            x="0"
            y="0"
            width="36"
            height="36"
            transform="translate(4 4) rotate(340 18 18) scale(1.1)"
            fill="#dbdffd"
            rx="36"
          ></rect>
          <g transform="translate(-4 -3) rotate(0 18 18)">
            <path
              d="M15 20c2 1 4 1 6 0"
              stroke="#000000"
              fill="none"
              stroke-linecap="round"
            ></path>
            <rect
              x="14"
              y="14"
              width="1.5"
              height="2"
              rx="1"
              stroke="none"
              fill="#000000"
            ></rect>
            <rect
              x="20"
              y="14"
              width="1.5"
              height="2"
              rx="1"
              stroke="none"
              fill="#000000"
            ></rect>
          </g>
        </g>
      </svg>
    </div>
  </section>
</template>

<script>
export default {
  name: "RightChatter",
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
.right {
  display: flex;
  flex-direction: row;
  justify-content: flex-end;
  align-items: center;
  width: 75vw;
  color: var(--background-color);
  font-family: var(--text-chat);
  font-size: 0.7rem;
}
.bubble-right {
  background-color: var(--svg-two);
  width: 200px;
  height: 50px;
  border-radius: 30px;
  text-align: center;
}
svg {
  height: 40px;
  width: auto;
  margin-top: 2rem;
}
p {
  margin-top: 1rem;
}
@media only screen and (min-width: 1000px) {
  .right {
    width: 37vw;
  }
}
@media only screen and (min-width: 1400px) {
  svg {
    height: 55px;
  }
  .bubble-right {
    width: 300px;
    height: 75px;
  }
  p {
    font-size: 1.1rem;
    margin-top: 1.7rem;
  }
  .right {
    width: 500px;
  }
}
</style>
