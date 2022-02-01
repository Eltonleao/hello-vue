<template>
  <Card></Card>
  <Card>lorem ipsum dolor sit amet</Card>
  <Card><h1>Hello World</h1></Card>
  <Card><img src="https://picsum.photos/500/100" alt="" srcset=""></Card>
</template>

<script>

import Card from "./components/Card.vue";

export default {
  methods:{
  },
  computed: {},
  watch: {},
  components:{
    Card
  }
}
</script>


<style>
  *{
    font-family: 'Courier New', Courier, monospace;
  }

</style>