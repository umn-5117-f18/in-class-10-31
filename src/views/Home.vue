<template>
  <div class="home">
    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
    <!-- <simple-template the-name="hi" /> -->
    <conditional-and-loop />

  </div>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from '@/components/HelloWorld.vue'
// import SimpleTemplate from '@/components/SimpleTemplate.vue';
import ConditionalAndLoop from '@/components/ConditionalAndLoop.vue';

export default {
  name: 'home',
  components: {
    // HelloWorld,
    // SimpleTemplate,
    ConditionalAndLoop
  }
}
</script>

