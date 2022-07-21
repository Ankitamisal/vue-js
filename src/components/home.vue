<template>
<!-- <h1>Name.....!{{Name}}</h1>
<h1>Email.....!{{email}}</h1>
<h1>Mobile ....!{{Mobile}}</h1>
<h1>Mobile ....!{{Mobile==8888}}</h1>
<h1>company....!{{getName('geoSpoc')}}</h1> -->
<!-- <h1 v-on:mousemove="getConsole()">Home</h1>
<button v-on:click="getData()">Click Me!</button>

<h2>{{count}}</h2> -->
<h2>pass data to child</h2>
<ChildPage name="ankita" :user="user" :getData="getData"/>

</template>

<script>
import ChildPage from './childPage.vue'
export default {
    name: "homePage",
       components: { ChildPage },
    data() {
        return {
            /*  count:0 */
            user:
        
        {
            name: "peter",
                email:
            "ankia@est.com"
        }
    }
 
},
    methods:{
getData()
{
    console.log("parent function called")
//   this.count=this.count+1;
}
/* getConsole()
{
    console.warn("function called");
} */
 }
}

</script>

<style scoped>
h1{
    color: orange;
}
</style>