<template>
  <div id="app">
    <img src="./assets/logo.png">
    <Excercise1 />
  </div>
</template>

<script>
import Excercise1 from './components/Excercise1'

export default {
  name: 'App',
  components: {
    Excercise1
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
