<template>
  <div id="app">
    <Header/>
    <HelloWorld/>
    <Card v-bind:Card="Card"/>
    <homepage/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld'
import Card from './components/Card'
import homepage from './components/homepage'
import Header from './components/Header'

export default {
  name: 'App',
  components: {
    homepage,
    Header
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
  padding: 0;
}

*{
  margin: 0;
}

</style>
