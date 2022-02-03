<template>

<h2 @mouseover="incrementCount">Hovered {{ count }} times</h2>
  
</template>

<script>
export default {
    name: "HoverCounter",
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