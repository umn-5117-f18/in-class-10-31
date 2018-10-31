<template>
  <div class="home">
    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
    <!-- <simple-template the-name="hi" /> -->
    <!-- <conditional-and-loop /> -->
    <!-- <user-input/> -->
    <computed-properties/>

  </div>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from '@/components/HelloWorld.vue'
// import SimpleTemplate from '@/components/SimpleTemplate.vue';
// import ConditionalAndLoop from '@/components/ConditionalAndLoop.vue';
// import UserInput from '@/components/UserInput.vue';
import ComputedProperties from '@/components/ComputedProperties.vue';

export default {
  name: 'home',
  components: {
    // HelloWorld,
    // SimpleTemplate,
    // ConditionalAndLoop,
    // UserInput,
    ComputedProperties
  }
}
</script>

