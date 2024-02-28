<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to my calculator in Vue.js! 😊"/>
  <CalculadoraAritimetica />
  <CalculadoraAritimeticaTwoo />
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import CalculadoraAritimetica from "./components/CalculadoraAritimetica.vue";
import CalculadoraAritimeticaTwoo from "./components/CalculadoraAritimeticaTwoo.vue";

export default {
  name: 'App',
  components: {
    HelloWorld,
    CalculadoraAritimetica,
    CalculadoraAritimeticaTwoo,
  },
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
