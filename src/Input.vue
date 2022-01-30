<template>
    <input type="text" v-model="name">
</template>

<script>
export default{
    name : "Input",
    data(){
        return {
            name : "",
        }
    },
}
</script>

<style>
    *{
        font-family: 'Courier New', Courier, monospace;
    }
    input{

    }
</style>