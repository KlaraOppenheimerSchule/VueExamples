<script setup>
import { ref } from 'vue'
import ChildComponentOne from './ChildComponentOne.vue';
import ChildComponentTwo from './ChildComponentTwo.vue'

const childMsgFromParent=ref("HelloToChild2")
const childMsg = ref('No child msg yet')


</script>

<template>
    <!-- The parent can pass the prop to the child just like attributes. To pass a dynamic value, we can also use the v-bind syntax:-->
    <ChildComponentTwo :childMsgFromParent="childMsgFromParent"></ChildComponentTwo>

    <!-- The Parent can catch message from child -->
    <ChildComponentOne  @childMsgFromChild="(msg) => childMsg = msg"></ChildComponentOne>
    <p>{{ childMsg }}</p>
</template>