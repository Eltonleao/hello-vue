<template>
<ul>
  <li v-for="item in computedItems" :key="item">{{item}}</li>
</ul>
</template>

<script>

export default {
  data() {
    return {
      items : [
        1,2,3,4,5
      ]
    }
  },
  methods:{
  },
  computed: {
    computedItems(){
      return this.items.filter(item => item > 2 && item < 5);
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
