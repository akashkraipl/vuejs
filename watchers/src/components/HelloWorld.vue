<script>
export default {
  name: "HelloWorld",
  data(){
    return {
      count: 0
    }
  },
  watch: {
    count(val, prev){
      if(val < 0){
        alert("Value can not be less then zero")
      }
    }
  }
}
</script>

<template>
  <h1>Watchers</h1>
  <h2>Count :- {{ count }}</h2>
  <button @click="count = count + 1">Increment</button>
  <button @click="count = count - 1">Decrement</button>
</template>
