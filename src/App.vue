<template>
  <div id="app">
    <!-- <img width="25%" src="./assets/logo.png">
    <HelloWorld msg="Hello Vue in CodeSandbox!" />-->
    <div class="draggable box" v-on:click="drag"></div>
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld";

export default {
  name: "App",
  components: {
    HelloWorld
  },
  methods: {
    drag: function(event) {
      console.log(event);
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
.box {
  background: green;
  height: 50px;
  position: absolute;
  top: 0;
  left: 0;
  width: 50px;
}
</style>
