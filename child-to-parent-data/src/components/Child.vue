<script>
export default {
    name: "Child",
    props: {
        getName: Function
    },
    data(){
        return {
            name: "Aakash"
        }
    }
}
</script>

<template>
    <button @click="getName(name)">Send</button>
</template>