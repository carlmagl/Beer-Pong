<template>
  <div id="app">
    <img src="./assets/logo.png">
    <HelloWorld/>
    <Card/>
    <homepage/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld'
import Card from './components/Card'

import homepage from './components/homepage'

export default {
  name: 'App',
  components: {
    HelloWorld,
    Card,
    homepage
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
*{
  margin: 0;
  padding: 0;
}

</style>
