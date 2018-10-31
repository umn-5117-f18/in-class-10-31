<template>
  <div class="home">
    <hr><h1>simple</h1>
    <simple-template the-name="hi" />
    <hr><h1>conditional and loop</h1>
    <conditional-and-loop />
    <hr><h1>user input</h1>
    <user-input/>
    <hr><h1>computed properties</h1>
    <computed-properties/>
    <hr><h1>parent/child communication</h1>
    <parent-component/>
    <hr><h1>slots</h1>
    <slot-component>
      <h1>hi, I am inside.</h1>
    </slot-component>

  </div>
</template>

<script>
import SimpleTemplate from '@/components/SimpleTemplate.vue';
import ConditionalAndLoop from '@/components/ConditionalAndLoop.vue';
import UserInput from '@/components/UserInput.vue';
import ComputedProperties from '@/components/ComputedProperties.vue';
import ParentComponent from '@/components/ParentComponent.vue';
import SlotComponent from '@/components/SlotComponent.vue';

export default {
  name: 'home',
  components: {
    SimpleTemplate,
    ConditionalAndLoop,
    UserInput,
    ComputedProperties,
    ParentComponent,
    SlotComponent,
  }
}
</script>

