<template>
  <div id="app">
    {{ name }}
    <button @click="alertAdd()">Add</button>
    <button @click="alertSub()">Sub</button>
    <input type="text" :value="item" />
    <img alt="Vue logo" src="./assets/logo.png" width="25%" />
    <HelloWorld msg="Hello Vue in CodeSandbox!" />
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld";

export default {
  name: "App",
  components: {
    HelloWorld,
  },
  data() {
    return {
      name: "teste",
      item: 1,
    };
  },
  methods: {
    alertAdd() {
      // this.age++;
      this.item++;
    },
    alertSub() {
      // this.age++;
      this.item--;
    },
  },
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
