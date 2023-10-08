<script>
export default {
  name: "HelloWorld",
  beforeCreate(){
    // we can not change the value of data because values are not exist upto now
    alert("Before created")
  },
  created(){
    alert("created")
  }
}
</script>

<template>
  <h1>Before created and created</h1>
</template>
