<script>
import Child from './Child.vue';
export default {
  components: { Child }
}
</script>

<template>
  <h1>Slots</h1>
  <h2>we want to send dynamic html content to child component</h2>
  <Child>
    <h1>Hello</h1>
  </Child>
  <!-- <Child><a href="google.com" target="_blank">Go to google</a></Child> -->
  <Child>
    <template v-slot:first>
      <h1>Named slot</h1>
    </template>
    <template v-slot:second>
      <h2>Named slot 2</h2>
    </template>
  </Child>
</template>
