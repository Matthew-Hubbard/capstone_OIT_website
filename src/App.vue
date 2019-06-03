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
  margin-top: 30px;
}

  body {
    /*background-image: url('~@/assets/design-development-electronics-326424.jpg');*/
    background-image: url('~@/assets/america-analysis-cellphone-926987.jpg');

    /* Background image is centered vertically and horizontally at all times */
    background-position: center center;

    /* Background image doesn't tile */
    background-repeat: no-repeat;

    /* Background image is fixed in the viewport so that it doesn't move when
       the content's height is greater than the image's height */
    background-attachment: fixed;

    /* This is what makes the background image rescale based
       on the container's size */
    background-size: cover;

    /* Set a background color that will be displayed
       while the background image is loading */
    background-color: #464646;
  }
</style>
