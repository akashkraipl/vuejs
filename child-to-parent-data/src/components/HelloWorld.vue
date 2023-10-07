<script>
import Child from './Child.vue';
export default {
  methods: {
    getName(name) {
      alert(name);
    }
  },
  components: { Child }
}
</script>

<template>
  <h1>Child to parent data transfer</h1>
  <Child :getName="getName" />
</template>
