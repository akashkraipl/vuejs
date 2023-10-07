<script>
export default {
    name: "Child",
    props: {
        name: String,
        user: Object,
        getData: Function
    }
}
</script>

<template>
    <h2>{{ name }}</h2>
    <h2>{{ user.name }}</h2>
    <button @click="getData()">Click me</button>
</template>