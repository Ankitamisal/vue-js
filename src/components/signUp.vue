<template>
<h3>sign up</h3>
<input type="text" placeholder="enter name">
<input type="text" placeholder="enter mail">
<input type="password" placeholder="enter password">
<button>Sign Up</button>
</template>

<script>
export default {
    name:'signUp',
}
</script>

<style>
input {
    width: 300px;
    margin-top: auto;
    margin-right: auto;
    margin: 10px;
    padding: 5px;
    display: block;
}
button
{
    margin-left: auto;
    margin-right: auto;
    width: 150px;
    height: 50px;
    background-color:red;
    margin-bottom: 25px;

}
</style>