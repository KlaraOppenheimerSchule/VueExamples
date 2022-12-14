<script setup>
    //In addition to receiving props, a child component can also emit events to the parent:
    const emit = defineEmits(['childMsgFromChild'])
    emit('childMsgFromChild', 'hello from childOne')
</script>

<template>
    <h1> I am the child one</h1>
</template>