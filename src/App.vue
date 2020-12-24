<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
    <button @click="increment">X</button>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import { mapMutations } from 'vuex'

export default {
  name: 'App',
  components: {
    HelloWorld
  },
  methods: {
  method2() {
    console.log('method2')
  },
  ...mapMutations(['increment'])
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
