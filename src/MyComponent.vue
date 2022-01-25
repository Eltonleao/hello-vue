<template>
<h2>
    {{teste}}
</h2>

</template>
<script>

export default{
    name: "MyComponent",
    data: function(){
        return {
            teste: 'lorem'
        }
    }
}

</script>


<style scoped>
h2{
    color: red;
}
</style>