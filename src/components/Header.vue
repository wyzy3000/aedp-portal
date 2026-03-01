<script setup lang="ts">
</script>

<template>
  <header class="header">
    <div class="container header-content">
      <div class="logo">
        <img src="../assets/aedp-logo.png" alt="AEDP Logo" />
      </div>
      <button class="btn-primary">About AEDP</button>
    </div>
  </header>
</template>

<style scoped>
.header {
  padding: 1.5rem 0;
  border-bottom: 1px solid #eaeaea;
}

.header-content {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.logo img {
  height: 72px; /* Increased by 20% from 60px */
  object-fit: contain;
}
</style>
