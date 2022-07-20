

<script>
import HelloWorld from './components/HelloWorld.vue'
/* import homePage from './components/home.vue'; */
import signUp from './components/signUp.vue';

export default {
  name: 'App',
  components: {
     HelloWorld, 
   /*  homePage, */
    signUp
  }
}
</script>

<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to vue.js"/>
 <!--  <homePage/> -->
  <signUp/>
</template>
