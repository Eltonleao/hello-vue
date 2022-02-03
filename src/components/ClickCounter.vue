<template>

<button @click="incrementCount">Clicked {{ count }} times</button>
  
</template>

<script>
export default {
    name: "ClickCounter",
    data(){
        return{
            count: 0
        }
    },
    methods:{
        incrementCount(){
            this.count++;
        }
    }

}
</script>

<style>

</style>