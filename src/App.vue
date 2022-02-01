<template>
  <Card>
    <template v-slot:header>
      <h3>Header</h3>
    </template>
    <template v-slot:default>
      <img src="https://picsum.photos/200" >
    </template>

    <template v-slot:footer>
      <h3>Footer</h3>
    </template>
  </Card>
  
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