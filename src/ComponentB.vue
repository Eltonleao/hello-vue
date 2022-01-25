<template>
<h1>Hello {{username}}</h1>
    
</template>


<script>
export default{
    name: "ComponentB",
    inject: ['username'],
}
</script>