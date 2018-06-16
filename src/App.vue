<template>
  <div id="app">
    <Big />
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld'
import Events from './components/event'
import Big from './components/slots/big'

export default {
  name: 'App',
  components: {
    HelloWorld,
    Events,
    Big
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
