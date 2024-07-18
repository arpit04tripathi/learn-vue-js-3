<script setup>
import { RouterView } from 'vue-router'
import FooterComponent from '@/components/_layouts/FooterComponent.vue'
import HeaderComponent from '@/components/_layouts/HeaderComponent.vue'
</script>

<template>
  <HeaderComponent>
    <!-- <template #heading>Tooling</template>
    <p>This fills up the slot</p> -->
  </HeaderComponent>

  <main class="container my-3">
    <RouterView />
  </main>

  <FooterComponent />
</template>

<style scoped></style>
