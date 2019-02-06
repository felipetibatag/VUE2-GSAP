<template>
  <div id="app" ref="box">
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";
import { TimelineLite } from "gsap";

export default {
  name: "app",
  components: {
    HelloWorld
  },
  mounted() {
    const { box } = this.$refs;
    const timeline = new TimelineLite();

    timeline.to(box, 1, { x: 200, rotation: 10, y: 100, rotation: 100 });
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
