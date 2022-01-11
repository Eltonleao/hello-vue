<template>
  <h2 v-for="(name, index) in names" v-bind:key="name">{{index}} - {{name}}</h2>
  
  <h2 v-for="name in fullNames" v-bind:key="name.first">
    <span v-if="show">
      {{name.first}} {{name.last}}
    </span>
  </h2>

  <div v-for="actor in actors" :key="actor.name">
    <h2>{{actor.name}}</h2>
    <ul v-for="movie in actor.movies" :key="movie">
      <li>{{movie}}</li>
    </ul>
  </div>

  <h2 v-for="(value, key, index) in myInfo" :key="value">{{index}} - {{key}} : {{value}}</h2>
  
</template>

<script>

export default {
  name: 'App',
  data() {
    return {
      show: false,
      names: ["lorem", "ipsum", "dolor"],
      fullNames : [
        {first: "lorem", last: "ipsum"},
        {first: "dolor", last: "sit"}
      ],
      actors: [
        {
          name: "Christian Bale",
          movies: ['Batman', "çldskjlfd"]
        },
        {
          name: "Di Caprio",
          movies: ['titanic', 'lkcsjhfdskl']
        }
      ],
      myInfo :{
        name: "ELton",
        ksjdf: "kasjhflsa",
        lskdjf: "lkds"
      }

      
    }
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
