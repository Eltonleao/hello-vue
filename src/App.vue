<template>
  <Article title="a" :likes="50" :published="true"></Article>

</template>

<script>

import Article from './Article.vue';

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

    Article
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
