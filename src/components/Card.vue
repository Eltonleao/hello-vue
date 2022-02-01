<template>
  <div class="card">
    <div id="card-header">
        <slot name="header"></slot>
    </div>
    <div id="card-content">
        <slot name="default"></slot>
    </div>
    <div id="card-footer">
        <slot name="footer"></slot>
    </div>
  </div>
</template>

<script>
export default {
  name: "Card",
  props: ["content"],
};
</script>


<style scoped>
.card {
    margin: 30px auto;
  width: 500px;
  height: 100px;
  text-align: center;
  display: flex;
  position: relative;
  justify-self: center;
  align-content: center;
  padding: 16px;
  box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
}
</style>