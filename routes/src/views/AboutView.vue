<script>
import { useRoute } from 'vue-router';
export default{
  data(){
    return {
      id: 0
    }
  },
  mounted(){
    const route = useRoute();
    this.id = route.params.id;
  }
}
</script>

<template>
  <div class="about">
    <h1>This is an about page {{ id }}</h1>
  </div>
</template>

<style>
@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
}
</style>
