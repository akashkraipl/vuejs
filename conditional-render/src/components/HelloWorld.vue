<script>
export default {
  data() {
    return {
      flag: true
    }
  },
  methods: {
    toggle() {
      this.flag = !this.flag;
    }
  }
}
</script>

<template>
  <h1 v-if="flag">If true</h1>
  <h1 v-else>Else</h1>
  <button @click="toggle">Toggle</button>
</template>
