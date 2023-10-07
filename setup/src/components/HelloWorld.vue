<!-- <script setup>
defineProps({
  msg: {
    type: String,
    required: true
  }
})
</script> -->

<script>
export default {
  props: {
    msg: {
      type: String,
      default: 'vertical',
      required: false
    },
  },
  page: {
    title: 'Test',
    meta: [
      { name: 'description', content: `test content` },
    ],
  },
  data() {
    return {
      email: "aakash@gmail.com",
      getName: function (a) {
        return a;
      },
      number: 9999
    }
  },
  methods: {
    getAge() {
      return 11
    },
    getData() {
      return {
        a: 1,
        b: 2,
        email: this.email
      }
    }
  }
}
</script>

<template>
  <div class="greetings">
    <h1 class="green">{{ msg }} {{ email }} {{ getName("Aakash") }} {{ number = 1111 }}</h1>
    <h2>{{ getAge() }}</h2>
    <h2>{{ getData().a }}</h2>
    <h2>{{ getData().email }}</h2>
  </div>
</template>

