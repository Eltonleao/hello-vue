<template>
  <h2>{{count}}</h2>
  <button v-on:click="increment()">add</button>
  <button v-on:click="decrement()">sub</button>

</template>

<script>

export default {
  data() {
    return {
      count: 0,
      name : "Yoda"
    }
  },
  methods:{
    increment(){
      this.count++;
    },
    decrement(){
      this.count--;
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
