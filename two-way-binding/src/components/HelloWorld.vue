<!-- <script setup>


</script> -->

<script>
export default {
  data() {
    return {
      name: "",
      email: "",
      skills: [],
      gender: null
    }
  }
}

</script>

<template>
  <input type="text" name="name" id="name" placeholder="name" v-model="name">
  <input type="email" name="email" id="email" placeholder="email" v-model="email">
  <label for="node">Node</label>
  <input type="checkbox" name="node" id="node" v-model="skills" value="node">
  <label for="nest">Nest</label>
  <input type="checkbox" name="nest" id="nest" v-model="skills" value="nest">

  <label for="gender">Gender</label>
  <input type="radio" name="gender" id="male" value="male" v-model="gender">
  <input type="radio" name="gender" id="female" value="female" v-model="gender">
  <h1>Name - {{ name }}</h1>
  <h1>email - {{ email }}</h1>
  <h1>skills - {{ skills }}</h1>
  <h1>gender - {{ gender }}</h1>
</template>
