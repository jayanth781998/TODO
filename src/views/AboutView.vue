<script setup>
import { reactive, ref } from 'vue';
import TodoButton from "../components/TodoButton.vue"
let count=ref(0)
</script>
<template>
  <div class="about">
    <h1>This is Jayanths ToDo List</h1>
    <br>
    <br>
<TodoButton @click="count++">{{ count}}</TodoButton>
  </div>
</template>

<style>
@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: top;
    flex-direction: column;
  }
}
</style>
