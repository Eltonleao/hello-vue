<template>
  <button @click="getPosts">Load Posts</button>
  <h3 v-if="errorMsg">{{errorMsg}}</h3>
  <div v-for="post in posts" :key="post.id">
      <h3>{{post.title}}</h3>
      <p>{{post.body}}</p>
      <hr>
  </div>
</template>

<script>
import axios from 'axios';

export default {
    name: "PostList",
    data(){
        return{
            posts: [],
            errorMsg: "",
        }
    },
    methods: {
        getPosts(){
            this.loading = true;
            console.log('lksajh');
            axios.get('https://jsonplaceholder.typicode.com/posts')
            .then(response => {
                this.posts = response.data;
                this.loading = false;
            })
            .catch(error => {
                console.log('entrei aqui');
                console.log(error);
                this.errorMsg = "oh no :(";
            })
        }
    },

}
</script>

<style>
</style>