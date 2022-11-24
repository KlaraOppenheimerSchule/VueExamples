<script setup>
    const props = defineProps({
        childMsgParent: String
    })

</script>

<template>
    <h1> {{childMsgParent}} </h1>
</template>