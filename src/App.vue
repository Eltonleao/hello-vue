<template>
  <button @click="active = 'TabA'">TabA</button>
  <button @click="active = 'TabB'">TabB</button>
  <button @click="active = 'TabC'">TabC</button>

  <keep-alive>
    <component :is="active"/>
  </keep-alive>
  <!-- <tab-a v-if="active == 'TabA'"></tab-a>
  <tab-b v-if="active == 'TabB'"></tab-b>
  <tab-c v-if="active == 'TabC'"></tab-c> -->
</template>

<script>
import TabA from './components/tabs/TabA.vue';
import TabB from './components/tabs/TabB.vue';
import TabC from './components/tabs/TabC.vue';

export default {
  data(){
    return{
      active: "TabA"
    }
  },
  methods:{
  },
  computed: {},
  watch: {},
  components:{
    TabA,
    TabB,
    TabC
  }
}
</script>


<style>
  *{
    font-family: 'Courier New', Courier, monospace;
    text-align: center;
  }

</style>