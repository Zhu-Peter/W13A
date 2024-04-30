<template>
  <div id="app">
    <VueHeader/><VueBody/>
  </div>
</template>

<script>
import VueHeader from './components/VueHeader.vue'
import VueBody from './components/VueBody.vue'

export default {
  name: 'App',
  components: {
    VueHeader, VueBody
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
  margin-top: 60px;
}
</style>
