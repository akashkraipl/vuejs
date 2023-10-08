<script>
export default {
  name: "HelloWorld",
  data() {
    return {
      count: 0
    }
  },
  beforeUpdate() {
    console.log("before update", this.$refs["num"].textContent);
  },
  updated() {
    console.log("updated", this.$refs["num"].textContent);
  }
}
</script>

<template>
  <h1>Before update and updated</h1>
  <h2 ref="num">{{ count }}</h2>
  <button @click="count = count + 1">+</button>
</template>
