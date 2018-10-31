<template>
  <div class="parent">
    <h2>parent</h2>

    <input type="text" v-model="parentName">

    <p>parent name: {{ parentName }}</p>

    <child-component 
      v-bind:parentName="parentName"
      v-on:good-job="foundGoodJob"/>

    <p>your child says:</p>

    <ul>
      <li v-for="m in messages" :key="m.id">
        good job: {{ m }}
      </li>
    </ul>
  </div>
</template>

<script>
  import ChildComponent from '@/components/ChildComponent.vue';

  export default {
    components: {
      ChildComponent
    },
    data() {
      return {
        parentName: "Max",
        messages: []
      }
    },
    methods: {
      foundGoodJob(msg) {
        if (msg) {
          this.messages.push(msg);
        }
        
      }
    },
  }
</script>

<style scoped>
.parent {
  border: 1px solid gray;
}
</style>