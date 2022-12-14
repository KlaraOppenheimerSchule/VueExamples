<script setup>
    const emit = defineEmits(['response'])
    emit('response', 'hello from childOne')

    const props = defineProps({
        childMsgParent: String
    })

</script>

<template>
    <h1> I am the child </h1>
    <p> {{childMsgParent}}</p>
</template>