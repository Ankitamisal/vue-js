<template>
<h1>user component</h1>
<button v-on:Click="getUser(mail)">send User Name</button>
</template>

<script>
export default {
    name:"userPage",
    data(){
       return {
        mail: "ankita@est.com"
       }
    },
    props:
    {
        getUser:Function
    }
}
</script>

<style>
</style>