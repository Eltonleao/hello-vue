<template>
  <h3 v-for="name in names" :key="name.firstName">
    <slot :firstName="name.firstName" :lastName="name.lastName"></slot>
  </h3>
</template>

<script>
export default {
  name: "Card",
  data(){
    return {
      names : [
        {
          firstName: "John",
          lastName: "Doe"
        },
        {
          firstName: "Jane",
          lastName: "Doe"
        },
        {
          firstName: "Joe",
          lastName: "Doe"
        },
        {
          firstName: "Jack",
          lastName: "Doe"
        }
      ]
    }
  }
};
</script>


<style scoped>

</style>