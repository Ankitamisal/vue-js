<template>
<!-- <h1>Name.....!{{Name}}</h1>
<h1>Email.....!{{email}}</h1>
<h1>Mobile ....!{{Mobile}}</h1>
<h1>Mobile ....!{{Mobile==8888}}</h1>
<h1>company....!{{getName('geoSpoc')}}</h1> -->
<h1 v-on:mousemove="getConsole()">Home</h1>
<button v-on:click="getData()">Click Me!</button>

<h2>{{count}}</h2>

</template>

<script>
export default {
    name:'homePage',
    data()
    {
         return{
            count:0
         }
    },
    methods:{
getData()
{
  this.count=this.count+1;
},
getConsole()
{
    console.warn("function called");
}
 }
}
</script>

<style scoped>
h1{
    color: orange;
    text-align: center;
}
</style>