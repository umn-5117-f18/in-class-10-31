<template>
  <div class="slot-component">
    <h1>slots allow you to put stuff inside a component</h1>
    <div class="inner">
      <slot></slot>
    </div>
  </div>
</template>

<script>
  export default {
    
  }
</script>

<style scoped>
.inner {
  border: 1px solid grey;
  padding: 10px;
}
</style>