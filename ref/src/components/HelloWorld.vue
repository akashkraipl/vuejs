<script>
export default {
  methods: {
    getData() {
      this.$refs.input.focus();
      // this.$refs.input.value    to get the value 
      // this.$refs.input.style.color = "red"    to change style 
    }
  }
}
</script>

<template>
  <h1>ref</h1>
  <input type="text" ref="input">
  <button @click="getData()">Click me</button>
</template>
