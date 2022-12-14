<script setup>
    const props = defineProps({
        childMsgFromParent: String
    })
</script>

<template>
    <h1> {{childMsgFromParent}} </h1>
</template>