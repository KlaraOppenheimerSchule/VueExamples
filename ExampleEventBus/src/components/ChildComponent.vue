<script setup>
    const props = defineProps({
        name: String
    })

</script>

<template>
    <h1> {{name}} </h1>
    <button @increase-by="increaseCount">click me</button>
</template>