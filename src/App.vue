<script setup lang="ts">
</script>

<template>
  <div class="container">
    <header>
      <h1>AEDP-portal</h1>
    </header>
    <main>
      <router-view></router-view>
    </main>
  </div>
</template>

<style scoped>
.container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 2rem;
  text-align: center;
}
header h1 {
  font-size: 3rem;
  color: #42b883;
  margin-bottom: 2rem;
}
</style>
