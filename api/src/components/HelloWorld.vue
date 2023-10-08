<script>
import axios from 'axios';

export default {
  name: "HelloWorld",
  data() {
    return{
      todos: []
    }
  },
  mounted() {
    axios.get("https://jsonplaceholder.typicode.com/todos").then((data) => { this.todos = data.data })
  }
}
</script>

<template>
  <h1>API</h1>
  <ul>
    <li v-for="item in todos" :key="item.id">{{ item.title }}</li>
  </ul>
</template>
