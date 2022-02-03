<template>

<h2 @mouseover="incrementCount">Hovered {{ count }} times</h2>
  
</template>

<script>

import mixin from '../mixins/counter.js';

export default {
    name: "HoverCounter",
    mixins: [mixin]

}
</script>

<style>

</style>