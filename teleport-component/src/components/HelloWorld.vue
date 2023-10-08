<script>
import Footer from './Footer.vue';
export default {
  name: "HelloWorld",
  components: {Footer}
}
</script>

<template>
  <h1>Teleport compoenent</h1>
  <p>everthing is injected in div with id app</p>
  <p>if we want to inject any other code outside of this then we use teleport</p>
  <telepost to="#footer"><Footer /></telepost>
</template>
