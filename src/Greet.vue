<template>
<h3>Hello {{name}}</h3>
<p>sua mensagem</p>
<p>{{message}}</p>

</template>

<script>

export default {
  name: "Teste",
  data() {},
  methods:{},
  computed: {},
  watch: {},
  props: ['name', 'message'],
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
