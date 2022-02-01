<template>
  <name-list>
    <template v-slot:default="slotProps">
      {{slotProps.lastName}}, {{slotProps.firstName}}
    </template>
  </name-list>
</template>

<script>

import NameList from "./components/NameList.vue";

export default {
  methods:{
  },
  computed: {},
  watch: {},
  components:{
    NameList
  }
}
</script>


<style>
  *{
    font-family: 'Courier New', Courier, monospace;
    text-align: center;
  }

</style>