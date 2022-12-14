<script setup>
import { ref } from 'vue'
import ChildComponent from './ChildComponent.vue';
import ChildComponentTwo from './ChildComponentTwo.vue'

const myName=ref("Klaus")

const childMsg = ref('No child msg yet')

function increaseCount(n) {
  count.value += n
}

</script>

<template>
    <ChildComponent  @response="(msg) => childMsg = msg" @response2="increaseCount"></ChildComponent>
    <p>{{ childMsg }}</p>
    <ChildComponentTwo :name="myName"></ChildComponentTwo>
</template>