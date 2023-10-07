<script>
export default {
    name: "Child",
    inheritAttrs: false
}
</script>

<!-- we are getting id from parent but not accepted as props so it by default attach to parent element  -->
<!-- if we want to bind with any other element then we use v-bind="$attrs"  -->
<!-- v-bind="$sttrs" when we use this then non props data attach to both parent and the element so  -->
<!-- we have to pass inheritAttrs: false to export default  -->
<template>
    <div>
        <h2 v-bind="$attrs">Hello</h2>
        <h2>Hii</h2>
    </div>
</template>