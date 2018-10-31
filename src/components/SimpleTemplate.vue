<template>
  <div class="simple-template">
    <p>message: {{ message }}</p>
    <p>message: <span v-html="message"/></p>
    <p>name: {{ theName }}</p>
    <p>now: {{ now }}</p>
    <span v-bind:title="now">hover over me</span>
  </div>
</template>

<script>
  export default {
    name: "simple-template",
    props: {
      theName: {
        type: String,
        default: "dude"
      },
    },
    data() {
      return {
        message: "<b>foo</b>",
        now: new Date().toLocaleString()
      }
    },
  }
</script>

<style scoped>

</style>