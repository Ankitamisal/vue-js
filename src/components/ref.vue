<template>
<!-- <div> -->
<h2>ref</h2>
<!-- <input type="text" ref="input"/>
<button v-on:click="getData">click me</button> -->
<!-- <ul>
    <li v-for="item in list" ref="items" :key="item">
        {{ item }}</li>
</ul>
</div> -->

    <p v-for="car in 4" ref="car" :key="car" >I am in car {{car}}</p>
    <button v-on:click="submit">view refs</button>

</template>

<script>
export default {
    name: 'refPage',
    data() {
        return {
            // list: [1, 3, 4]
        }
    },
    // mounted() {
    //     console.log(this.$refs.items);
    // },

    methods: {
        submit() {
            console.log(this.$refs['car'])
        }
        //     getData()
        //     {
        //         this.$refs.input.focus();
        //         let val=this.$refs.input.value
        //         console.log(val);
        //     }
        // }
    }
}
</script>

<style>
button {
    margin: 10px;
}
</style>
