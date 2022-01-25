<template>
<Greet></Greet>
<myComponent></myComponent>
</template>

<script>

import Teste from './Greet.vue';
import MyComponent from './MyComponent.vue';

export default {
  data() {
  },
  methods:{},
  computed: {},
  watch: {},
  components:{
    Greet: Teste,
    MyComponent: MyComponent
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
