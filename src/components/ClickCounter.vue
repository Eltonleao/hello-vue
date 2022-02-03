<template>

<button @click="incrementCount">Clicked {{ count }} times</button>
  
</template>

<script>

import mixin from '../mixins/counter.js';

export default {
    name: "ClickCounter",
    mixins: [mixin]

}
</script>

<style>

</style>