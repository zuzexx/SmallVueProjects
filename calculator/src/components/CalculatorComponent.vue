<template>
  <main>
    <section>
      <div class="calc-result">{{ calculatorValue }}</div>
      <div class="buttons-grid">
        <div class="buttons" v-for="button in calculatorButtons" :key="button">
          <div
            class="button-style"
            :class="{
              'bg-operators': ['C', '*', '/', '-', '+', '%', '='].includes(
                button
              ),
              'zero-button': [0, '='].includes(button),
            }"
            @click="buttonClick(button)"
          >
            {{ button }}
          </div>
        </div>
      </div>
    </section>
  </main>
</template>
<script>
export default {
  name: "CalculatorComponent",
  data() {
    return {
      calculatorValue: "",
      operator: null,
      previousValue: "",
      calculatorButtons: [
        "C",
        "*",
        "/",
        "-",
        7,
        8,
        9,
        "+",
        4,
        5,
        6,
        "%",
        1,
        2,
        3,
        ".",

        0,
        "=",
      ],
    };
  },
  methods: {
    buttonClick(button) {
      if (!isNaN(button) || button === ".") {
        this.calculatorValue += button + "";
      }
      if (button === "C") {
        this.calculatorValue = "";
      }
      if (button === "%") {
        this.calculatorValue = this.calculatorValue / 100 + "";
      }
      if (["/", "+", "*", "-"].includes(button)) {
        this.operator = button;
        this.previousValue = this.calculatorValue;
        this.calculatorValue = "";
      }
      if (button === "=") {
        this.calculatorValue = eval(
          this.previousValue + this.operator + this.calculatorValue
        );
        this.previousValue = "";
        this.operator = null;
      }
    },
  },
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
  font-family: "Open Sans", sans-serif;
}
section {
  border: 2px solid red;
  border-radius: 0.5rem;

  width: 500px;
  margin: 3rem, auto;
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 1rem;
}
.calc-result {
  padding: 1.2rem;
  width: 450px;
  border-radius: 0.5rem;
  text-align: right;
  border: 2px solid blue;
  font-weight: 700;
  font-size: 1.5rem;
}
.buttons-grid {
  display: flex;
  flex-wrap: wrap;
  width: 500px;
  justify-content: flex-start;
  align-items: center;
  margin-top: 1rem;
}
.button-style {
  text-align: center;
  margin: 0.25rem;
  width: 7.3rem;
  padding-top: 1.5rem;
  padding-bottom: 1.5rem;
  background-color: pink;
  border-radius: 0.5rem;
}
.button-style:hover {
  cursor: pointer;
  opacity: 0.8;
  transition: 0.7s;
}
.bg-operators {
  background-color: orange;
}

.zero-button {
  width: 15.1rem;
}
</style>
