<template>
  <div id="app">
    <HelloWorld msg="Capstone Spring 2019: OIT Web Apps"/>
<!--    <img alt="Vue logo" src="./assets/logo.png">-->
    <Backlog />
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import Backlog from './components/Backlog.vue'

export default {
  name: 'app',
  components: {
    HelloWorld,
    Backlog
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
