<script setup>
 import AlertComponent from './components/AlertComponent.vue';
 import { ref } from 'vue';

const time = ref('morning');
 

</script>

<template>
  <img alt="Vue logo" class="logo" src="./assets/logo.svg" width="125" height="125" />

  <div class="wrapper">
    <h1 v-if="time == 'morning'">Good Morning</h1>
    <h1 v-else-if="time == 'afternoon'">Good Afternoon</h1>
    <h1 v-else>Good Evening</h1>

  <div class = "btn">
    <button @click="time = 'morning'">Morning</button>
    <button @click="time = 'afternoon'">Afternoon</button>
    <button @click="time = 'evening'">Evening</button>
  </div>
  </div>

</template>

<style scoped>
button {
    padding: 10px;
    background-color: #007bff;
    color: #fff;
    border: none;
    border-radius: 5px;
    cursor: pointer;
}
.btn{
  display: flex;
  gap: 10px;
}

</style>
