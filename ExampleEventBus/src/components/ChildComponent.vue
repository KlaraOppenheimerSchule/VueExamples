<script setup>
    const emit = defineEmits(['response'])
    emit('response', 'hello from childOne')

</script>

<template>
    <h1> I am the child </h1>
</template>