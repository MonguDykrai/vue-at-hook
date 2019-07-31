<template>
  <div id="app">
    <!-- <img alt="Vue logo" src="./assets/logo.png"> -->
    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
    <Child @hook:mounted="childMounted" @hook:created="childCreated" />
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";
import Child from "@/components/Child";

export default {
  name: "app",
  components: {
    HelloWorld,
    Child
  },
  methods: {
    childMounted() {
      console.log(`childMounted`);
    },
    childCreated() {
      console.log(`childCreated`);
    }
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
