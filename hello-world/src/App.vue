<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld :msg="message"/>
  <input type="text" v-model="message"/>
  <button @click="alertMessage">Alert</button>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    HelloWorld
  },
  data(){
    return {
      message: 'Hello World!'
    }
  },
  methods: {
    alertMessage() {
      alert(this.message)
    }
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
