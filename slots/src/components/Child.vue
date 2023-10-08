<script>
export default {
    name: "Child"
}
</script>

<template>
    <div>
        <slot></slot>    <!-- slot without name-->
        <!-- <slot>Default text</slot>  slote with default text  -->

        <slot name="first"></slot>
        <slot name="second"></slot>
    </div>
</template>