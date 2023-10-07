<script>
export default {
  data(){
    return {
      data: ""
    }
  }
}
</script>

<template>
  <h1>Form modifiers</h1>
  <!-- v-model.lazy  it update the value when focus change of input  -->
  <!-- v-model.trim    it auto trim the value  -->
  <!-- v-model.number    convert value to number  -->

  <!-- v.model.lazy.number  chain form modifiers  -->
  
  <input type="text" v-model="data">
  <h2>{{ data }}</h2>
  <!-- <button @click="getData()">Click me</button> -->
</template>
