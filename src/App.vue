<script setup>
import AppHeader from './components/AppHeader.vue';
import AppFooter from './components/AppFooter.vue';
import AppCards from './components/AppCards.vue';
</script>

<template>
  <AppHeader></AppHeader>
  <AppCards></AppCards>
  <AppFooter></AppFooter>
</template>

<style lang="scss">
@use './styles/variables.scss' as *;
@use './styles/app.scss' as *;
</style>
