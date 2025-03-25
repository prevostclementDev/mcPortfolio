<script setup lang="ts">
import "~/assets/reset.css"
</script>

<template>
  <div class="container">
    <navbar />
      <div class="page">
        <NuxtPage />
      </div>
    <Footer />
  </div>
</template>

<style lang="scss" scoped>
.container {
  background: #000000;
  min-height: 100vh;

}
</style>