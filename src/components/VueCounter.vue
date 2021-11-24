<template>
  <div id="vue" class="counter">
    <button @click="subtract()">-</button>
    <pre>{{ count }}</pre>
    <button @click="add()">+</button>
  </div>
</template>

<script lang="ts" setup>
import { ref } from 'vue';

const count = ref(1);
const add = () => (count.value = count.value + 1);
const subtract = () => (count.value = count.value - 1);
</script>
