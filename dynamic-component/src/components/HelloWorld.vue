<script>
import Node from './Node.vue';
import Php from './Php.vue';
export default {
  name: "HelloWorld",
  components: { Node, Php },
  data(){
    return {
      tab: "Php"
    }
  }
}
</script>

<template>
  <h1>Dynamic components</h1>
  <component :is="tab" />
  <button @click="tab='Php'">Load php</button>
  <button @click="tab='Node'">Load node</button>
  <!-- <Php />
  <Node /> -->
</template>
