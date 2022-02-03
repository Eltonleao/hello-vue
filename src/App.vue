<template>
  <HoverCounter></HoverCounter>
  <ClickCounter></ClickCounter>
</template>

<script>

import ClickCounter from "./components/ClickCounter.vue";
import HoverCounter from "./components/HoverCounter.vue";

export default {
  data(){
    return{
      
    }
  },
  methods:{
  },
  computed: {},
  watch: {},
  components:{
    ClickCounter,
    HoverCounter
  }
}
</script>


<style>
  *{
    font-family: 'Courier New', Courier, monospace;
    text-align: center;
  }

</style>