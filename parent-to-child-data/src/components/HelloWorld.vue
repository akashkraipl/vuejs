<script>
import Child from './Child.vue';

export default {
  name: "Home",
  data() {
    return {
      user: { name: "Ram" },
      tag: "<h1>HTML Binding</h1>", // html binding (render text as html in vue js)
      isColor: true
    }
  },
  components: { Child },
  methods: {
    getData() {
      console.log("Parent function called");
    }
  },
  computed: {
    applyClass(){
      return {
        green: this.isColor,
        error: true,
        other: true
      }
    }
  }
}
</script>

<template>
  <h1 class="heading">Pass data from parent to child</h1>
  <Child name="Aakash" :user="user" :getData="getData" />

  <!-- html binding  -->
  <div v-html="tag"></div>

  <!-- dynamic class   -->
  <div :class="{ green: isColor }">Dynamic Class</div> <!-- { green: true } then apply this class  -->
  <!-- if any other class the we can give like this  -->
  <div class="other" :class="{ green: isColor }">Dynamic Class</div>

  <!-- if we have too many dynamic class then we give like this  -->
  <div :class="applyClass">Dynamic Class</div>
</template>

<style>
.heading {
  background-color: lightgreen;
}

.green {
  background-color: green;
}

.error{
  color: red;
}
</style>