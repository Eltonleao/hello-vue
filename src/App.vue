<template>
  <div>
    <pre>
      {{JSON.stringify(form, null, 2)}}
    </pre>

  </div>
  <form @submit="handleSubmit($event)">
    <label for="name">name: </label>
    <input type="text" id="name" v-model.trim="form.name">

    <input type="submit" value="submit">
  </form>  

</template>

<script>

export default {
  data() {
    return {
      form :{
        name: ""
      }
    }
  },
  methods:{
    handleSubmit($event){
      $event.preventDefault();
      console.log(this.form.name);
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
