<script>
export default {
  name: "HelloWorld",
  beforeMount(){
    console.log("before mount",this.$el);
  },
  mounted(){
    console.log("mount",this.$el);
  }
}
</script>

<template>
  <h1>Before mount and mounted</h1>
</template>
