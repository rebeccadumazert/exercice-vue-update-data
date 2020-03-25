<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png" />
    <!-- <HelloWorld msg="Welcome to Your Vue.js App" /> -->
    <ChangeBackground></ChangeBackground>
    <ClickClick></ClickClick>
    <SomeButtons></SomeButtons>
  </div>
</template>

<script>
// import HelloWorld from "./components/HelloWorld.vue";
import ChangeBackground from "./components/ChangeBackground";
import ClickClick from "./components/ClickClick";
import SomeButtons from "./components/SomeButtons";

export default {
  name: "App",
  components: {
    // HelloWorld,
    ChangeBackground,
    ClickClick,
    SomeButtons
  }
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
