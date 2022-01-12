<template>
<h2>{{add(2,2)}}</h2>
</template>

<script>

export default {
  data() {
    return {
      
    }
  },
  methods:{
    add(a, b){
      return a + b;
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
