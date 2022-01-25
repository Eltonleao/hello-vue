<template>
<h2>Volume Tracker (0-20)</h2>
<h3>Current Volume - {{volume}}</h3>
<div>
  <button v-on:click="volume -= 2 ">Decrease</button>
  <button v-on:click="volume += 2 ">Increase</button>
</div>

</template>

<script>

export default {
  data() {
    return {
      volume: 0
    }
  },
  methods:{},
  computed: {},
  watch: {
    volume: function(newVal, oldVal) {
    console.log("🚀 ~ file: App.vue ~ line 23 ~ oldVal", oldVal)
    console.log("🚀 ~ file: App.vue ~ line 23 ~ newVal", newVal)
      if (newVal > 60) {
        alert("Quer ficar surdo mlk?");
        this.volume = 60;
      } else if (newVal < 0) {
        this.volume = 0
      }
    }
  },
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
