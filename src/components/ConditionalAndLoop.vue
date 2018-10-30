<template>
  <div>

    <div v-if="a == 'dude'">YES</div>
    <div v-else>NO</div>
    
    <ul>
      <li v-for="i in l" :key="i">
        {{ i }}
      </li>
    </ul>

  </div>
</template>

<script>
  export default {
    data() {
      return {
        a: "dude",
        f: false,
        t: true,
        l: [1, 2, 3, 4],
        l2: []
      }
    },
    
  }
</script>
