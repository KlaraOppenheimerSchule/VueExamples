<script setup>
import { ref } from 'vue'
import ChildComponent from './ChildComponent.vue';

const myname=ref("Klaus")

function increaseCount(n) {
  count.value += n
}

</script>

<template>
    <ChildComponent :name="myname"></ChildComponent>
</template>