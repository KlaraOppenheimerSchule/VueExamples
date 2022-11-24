<script setup>
import { ref } from 'vue'
import ChildComponent from './ChildComponent.vue';
import ChildComponentTwo from './ChildComponentTwo.vue'

const myname=ref("Klaus")

const childMsg = ref('No child msg yet')

function increaseCount(n) {
  count.value += n
}

</script>

<template>
    <ChildComponent :name="myname" @response="(msg) => childMsg = msg" @response2="increaseCount"></ChildComponent>
    <p>{{ childMsg }}</p>
</template>