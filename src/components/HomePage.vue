<template>
<h2>ref data</h2>
<refPage/>
<SimpleForm/>
</template>

<script>
import refPage from './ref.vue'
import SimpleForm from './SimpleForm.vue'

export default {
    name:"HomePage1",
    components:{
    refPage,
    SimpleForm
}
}
</script>

<style></style>