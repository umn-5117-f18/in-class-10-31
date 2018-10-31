<template>
  <div>
    <p>{{ message }}</p>
    <button v-on:click="reverseIt">reverse</button>

    <p>
      <code>@click</code> is shorthand for <code>v-on:click</code>
    </p>

    <hr>

    <p>
      example of the <code>.prevent</code> modifier
    </p>

    <a href v-on:click.prevent="reverseIt()">click the link</a>

    <hr>

    <form class="pure-form ">
      <input type="text" placeholder="enter text"
             v-model="theText">
      <p>here's what you've entered: {{ theText }}</p>

      <input type="checkbox" id="checkbox" v-model="checked">
      <label for="checkbox">{{ checked }}</label>

    </form>

  </div>
</template>

<script>
  export default {
    data() {
      return {
        message: "hello, world",
        theText: null,
        checked: false,
        picked: null
      }
    },
    methods: {
      reverseIt() {
        this.message = this.message.split('').reverse().join('');
      }
    },
    
  }
</script>

