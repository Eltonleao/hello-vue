<template>
  <popup v-show="show" @close="handleClose"></popup>
  <button v-show="!show" @click="show = true">show</button>
</template>

<script>
import Popup from './Popup.vue';

export default {
  data() {
    return {
      show: false
    }
  },
  methods:{
    handleClose(msg){
      alert(msg);
      console.log(msg);
      return this.show = false;
    }
  },
  computed: {},
  watch: {},
  components:{
    Popup
  }
}
</script>


<style>
  *{
    font-family: 'Courier New', Courier, monospace;
  }

</style>