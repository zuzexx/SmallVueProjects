<template>
  <div>
    <TopComponent />
    <MiddleComponent />
    <BottomComponent />
  </div>
</template>

<script>
import TopComponent from "./components/TopComponent/TopComponent.vue";
import MiddleComponent from "./components/MiddleComponent/MiddleComponent.vue";
import BottomComponent from "./components/BottomComponent/BottomComponent.vue";
export default {
  name: "App",
  components: { TopComponent, MiddleComponent, BottomComponent },
};
</script>
