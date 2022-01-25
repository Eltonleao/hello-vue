<template>
<div>
    <h2>{{title}}</h2>
    <p>Likes: {{likes}}</p>
    <p>{{published ? 'published' : "not published"}}</p>
</div>
    
</template>

<script>

export default{
    name: "Article",
    props:{
        title: String,
        likes: Number,
        published: Boolean
    }

}
</script>
