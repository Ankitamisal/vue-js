<template>
<!-- <h1>Name.....!{{Name}}</h1>
<h1>Email.....!{{email}}</h1>
<h1>Mobile ....!{{Mobile}}</h1>
<h1>Mobile ....!{{Mobile==8888}}</h1>
<h1>company....!{{getName('geoSpoc')}}</h1> -->
<!-- <h1 v-on:mousemove="getConsole()">Home</h1>
<button v-on:click="getData()">Click Me!</button> -->
<h2>pass data to child Components</h2>
<childPage name="GeoSpoc" :user="user" :getData="getData" />

<!-- <h2>{{count}}</h2> -->
</template>

<script>
import childPage from './childPage.vue'
export default {
    name: "homePage",
    components: {
        childPage
    },
    data() {
        return {
            // count: 0,
            user: {
                name: 'ankita',
                email: 'anaw@g.com'
            }
        };
    },
    methods: {
        getData() {
            // this.count = this.count + 1;
            console.log("parent function called")

        },
        /*   getConsole() {
              console.warn("function called");
          } */
    },

}
</script>

<style scoped>
h2 {
    color: orange;
}
</style>
