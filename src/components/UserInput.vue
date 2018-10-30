<template>
  <div>
    <p>{{ message }}</p>
    <button v-on:click="reverseIt">reverse</button>

    <hr>

    <form class="pure-form">
      <input type="text" placeholder="enter text"
             v-model="theText">
      here's what you've entered: {{ theText }}
    </form>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        message: "hello, world",
        theText: null
      }
    },
    methods: {
      reverseIt() {
        this.message = this.message.split('').reverse().join('');
      }
    },
    
  }
</script>

