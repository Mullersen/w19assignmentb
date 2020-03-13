<template>
  <div id="app">
    <myHeader msg="This is a very majestic header"/>
    <myBody/>
    <myFooter msg="footer things for a footer"/>
  </div>
</template>

<script>
import myHeader from './components/Header.vue'
import myBody from './components/Body.vue'
import myFooter from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    myHeader,
    myBody,
    myFooter
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
