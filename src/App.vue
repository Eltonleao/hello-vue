<template>
  <h1>Hello {{name}}</h1>
  <div v-text="description"></div>
  <div v-html="html"></div>
  <span v-bind:class="status" class="teste">Status</span>
  <h2 v-bind:class="isPromoted && 'promoted'">Promoted</h2>
  <h2 v-bind:class="isSoldout ? 'soud-out': 'new'">Soudout</h2>
  <h2 v-bind:class="['new', 'promoted']">Newly promoted Movie</h2>
  <h2 v-bind:class="['new', isSoldout ? 'soud-out': 'new']">Array Conditional</h2>
  <h2 v-bind:class="{
    new: isSoldout,
    promoted: isPromoted
  }">Object Class Bind</h2>



  <h2 v-bind:style="{
    color: color,
    fontSize: size,
    border: border
  }">
    lorem ipsum
  </h2>

  <header>
    <h2 v-bind:style="headerStyleObj">Header</h2>
  </header>
   <p v-bind:style="[successStyleObj, badgeStyleObj]">nsldkfhdaskf</p>
</template>

<script>

export default {
  name: 'App',
  data() {
    return {
      name: "Dart",
      description: "lorem ipsum dolor sit amet",
      html: `<button onclick='alert("hey hey hey")'>lorem ispum</button>`,
      status: "danger",
      isPromoted: false,
      isSoldout: true,
      color: "red",
      size: "50px",
      border: 'solid green 2px',
      headerStyleObj : {
        color: 'green',
        fontSize: "100px"
      },
      successStyleObj : {
        backgroundColor: "green"
      },
      badgeStyleObj :{
        color: "red"
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

.promoted{
  font-style: italic;
}
.new{
  color: green;
}
</style>
