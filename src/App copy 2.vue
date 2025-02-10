<script setup>
import AlertComponent from './components/AlertComponent.vue';
</script>

<template>
  <img alt="Vue logo" class="logo" src="./assets/logo.svg" width="125" height="125" />

  <AlertComponent type="success" msg="This is a success alert" /><br>
  <AlertComponent type="danger" msg="This is a danger alert" /><br>
  <AlertComponent type="warning" msg="This is a warning alert" /><br>
  <alert-component type="info" msg="This is a info alert"/>
  <br>
  <alert-component />
</template>

<style scoped>
</style>
