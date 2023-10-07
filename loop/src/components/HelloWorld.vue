<script>
export default {
  data() {
    return {
      skills: ["Node", "Nest", "Vue"],
      users: [
        {
          name: "Ram"
        },
        {
          name: "Jon"
        }
      ]
    }
  }
}
</script>

<template>
  <h1>Skills</h1>
  <ul>
    <li v-for="item in skills" :key="item">{{ item }}</li>
  </ul>
  <h1>Users</h1>
  <ul>
    <li v-for="item in users" :key="item.name">{{ item.name }}</li>
  </ul>
</template>
