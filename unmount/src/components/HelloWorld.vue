<script>
import Child from './Child.vue';
export default {
  name: "HelloWorld",
  components:{Child},
  data(){
    return {
      isShow: true
    }
  }
}
</script>

<template>
  <h1>Before unmount and unmounted</h1>
  <button @click="isShow=!isShow">Toggle</button>
  <Child v-if="isShow" />
</template>
