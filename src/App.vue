<template>
  <ComponentA></ComponentA>  
</template>

<script>

import ComponentA from './ComponentA.vue';
export default {
  data() {
    return {
      username: 'John Doe'
    }
  },
  methods:{},
  computed: {},
  watch: {},
  components:{
    ComponentA
  },
  provide: function(){
    return {
      username: this.username
    }
  }
}
</script>