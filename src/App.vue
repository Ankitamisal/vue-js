

<script>
import HelloWorld from './components/HelloWorld.vue'
import homePage from './components/home.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    homePage
  }
}
</script>

<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to vue.js"/>
  <homePage/>
</template>
