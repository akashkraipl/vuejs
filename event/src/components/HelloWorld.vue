<!-- <script setup>
defineProps({
  msg: {
    type: String,
    required: true
  }
})
function say(message) {
  alert(message)
}

</script> -->

<script>
export default {
  data() {
    return {
      count: 0
    }
  },
  props: {
    msg: {
      type: String,
      default: "Hello"
    }
  },
  methods: {
    say(message) {
      alert(message)
    },
    increment() {
      this.count = this.count + 1;
    }
  }
}

</script>

<template>
  <div class="greetings">
    <h1 class="green">{{ msg }}</h1>
    <button @click="say('Hello')">Hello</button>
    <button v-on:click="say('Hello')">Hello 1</button>
    <button v-on:dblclick="say('Hello')">double click</button>
    <button @dblclick="say('Hello')">double click 1</button>
    <button @click="increment()">Increment</button>
    <h1>Count-- {{ count }}</h1>
  </div>
</template>
