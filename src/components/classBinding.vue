<template>
<h2>css Binding</h2>
<button type="button" class="red" v-on:click="getdata()" :getdata="getdata">Click me</button>

</template>

<script>

export default{
    name:'classBinding',
   methods:{
    getdata()
    {
alert('hello,fun friday!....')
    }
}
}
</script>

<style>
.red{
    background-color: red;
    margin: 20px;
    padding: 10px;
    border-radius: 2%;
    font-size: large;
}
.red:hover
{
    cursor: pointer;
}
</style>