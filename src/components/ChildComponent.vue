<template>
  <div class="child">
    <h2>child</h2>

    <p>child (parent is {{ parentName }})</p>

    <p>type a happy message:</p>
    <input type="text" v-model="msg" placeholder="well done, sir!">

    <button @click="$emit('good-job', msg)">click to say good job to {{ parentName }}</button>
    
  </div>
</template>

<script>
  export default {
    data() {
      return {
        msg: null
      }
    },
    props: {
      parentName: {
        type: String,
        default: null
      },
    }
  }
</script>

<style scoped>
.child {
  border: 1px solid green;
}
</style>