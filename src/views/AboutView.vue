<script setup lang="ts">
import TestBootstrap from '@/components/TestBootstrap.vue';
</script>

<template>
  <div class="about">
    <h1>This is an about page</h1>
  </div>
  <TestBootstrap/>
</template>

<style>
@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
}
</style>
