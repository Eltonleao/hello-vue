<template>

<template v-for="item in [1,2,3,4,5,6,7,8,9,10]" :key="item">
  <greet v-bind:name='name' message="lorem ipsum dolor sit amet"></greet>
</template>

</template>

<script>

import Teste from './Greet.vue';
// import MyComponent from './MyComponent.vue';

export default {
  data() {
    return{
      name: "Darth Vader"
    }
  },
  methods:{},
  computed: {},
  watch: {},
  components:{
    Greet: Teste
    // MyComponent: MyComponent
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
