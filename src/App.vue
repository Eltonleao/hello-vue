<template>
  <popup v-show="show" @close="show = false"></popup>
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
  methods:{},
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