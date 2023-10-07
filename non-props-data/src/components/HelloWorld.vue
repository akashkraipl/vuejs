<script>
import Child from './Child.vue';
export default {
  components: { Child }
}
</script>

<template>
  <h1>Non props data</h1>
  <!-- id we are sending to child  -->
  <Child id="1234" />
</template>
