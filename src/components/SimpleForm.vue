<template>
<h1>Simple Form</h1>
<form action="">
    <label for="">Email :</label>
    <input type="text" placeholder="enter email" v-model="form.email" />

    <label for="">Password :</label>
    <input type="password" placeholder="enter password" v-model="form.password" />

    <label for="">country</label>
    <select name="" id="" v-model="form.country">
        <option>India</option>
        <option value="">usa</option>
    </select>

    <label for="">Gender</label>
    <label for="">Male</label>
    <input type="radio" value="Male" id="" v-model='form.gender' />
    <label for="">Female</label>
    <input type="radio" value="Female" id="" v-model="form.gender" />

    <button type="button" v-on:click="login">Submit</button>
</form>
</template>

<script>
export default {
    name: 'SimpleForm',
    data() {
        return {
            form: {
                email: '',
                password: '',
                country: '',
                gender: ''

            },
            error:[],
        }
    },
    methods: {
        login() {
            this.error=[]
           for(const item in this.form)
           {
            if(this.form[item] ==='' || this.form[item].length===0) 
           {
            this.error.push(item)
           }
           }
           if(this.error.length===0)
           {
            alert('data submitted successfully')
           }
            console.log(this.form,this.error)
        }
    }
}
</script>

<style>
label {
    margin: 10px;
    padding: 5px;
    display: inline-block;
}
</style>
