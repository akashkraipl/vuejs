<script>
export default {
    name: "Child",
    beforeUnmount() {
        console.log("before unmount");
    },
    unmounted() {
        console.log("unmount");
    }
}
</script>

<template>
    <h1>Child</h1>
</template>