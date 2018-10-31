<template>
  <div>
    <p>message: {{ message }}</p>
    <p>message, spaced: {{ spacedMessage }}</p>

    <hr>

    <p>toggle: {{ toggle }}</p>
    <button class="pure-button" 
            v-bind:class="btnType"
            @click="toggleBtn()">click to toggle class</button>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        message: "hello, world",
        toggle: false
      }
    },
    computed: {
      spacedMessage() {
        return this.message.split("").join("__"); 
      },
      btnType() {
        return {
          "pure-button-primary": this.toggle
        }
      }
    },
    methods: {
      toggleBtn() {
        this.toggle = !this.toggle;
      }
    },
  }
</script>

<style scoped>

</style>