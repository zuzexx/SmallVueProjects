<template>
  <section class="left">
    <div class="avatar-left">
      <svg
        viewBox="0 0 36 36"
        fill="none"
        role="img"
        xmlns="http://www.w3.org/2000/svg"
        width="80"
        height="80"
      >
        <title>Nellie Bly</title>
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
          <rect width="36" height="36" fill="#dbdffd"></rect>
          <rect
            x="0"
            y="0"
            width="36"
            height="36"
            transform="translate(8 8) rotate(118 18 18) scale(1.1)"
            fill="#b3e8e5"
            rx="6"
          ></rect>
          <g transform="translate(4 4) rotate(-8 18 18)">
            <path d="M13,20 a1,0.75 0 0,0 10,0" fill="#000000"></path>
            <rect
              x="11"
              y="14"
              width="1.5"
              height="2"
              rx="1"
              stroke="none"
              fill="#000000"
            ></rect>
            <rect
              x="23"
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
    <div class="bubble-left">
      <p>{{ text }}</p>
    </div>
  </section>
</template>

<script>
export default {
  name: "LeftChatter",
  props: {
    text: {
      type: String,
      required: true,
    },
  },
};
</script>
<style scoped>
.left {
  display: flex;
  flex-direction: row;
  justify-content: flex-start;
  align-items: center;
  width: 80vw;
  color: var(--background-color);
  font-family: var(--text-chat);
  font-size: 0.7rem;
}
.bubble-left {
  background-color: var(--svg-three);
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
</style>
