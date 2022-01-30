<template>
    <div id="popup">
        <h2>This is a popup{{name}}</h2>
        <input type="text" v-model="name">
        <a @click="$emit('close', name)"> close</a>
    </div>
</template>

<script>
export default{
    name: "Popup",
    emits: {
        close: (name) =>{
            return !!name;
        }
    },
    data(){
        return{
            name: ""
        }
    }
}
</script>


<style>
#popup{
    display: flex;
    justify-content: center;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: rgba(0,0,0,0.5);
    z-index: 999;
}
</style>