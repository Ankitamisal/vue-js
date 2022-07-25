<template>
<h2>HTML BINDING</h2>
<div v-html="tag">

</div>
</template>
<script>
export default{
    name:'BindingPage',
    data(){
        return {
            tag:"<h2>hello html</h2>"
        }
    }
}
</script>
<style></style>