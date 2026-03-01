<script setup lang="ts">
import Header from '../components/Header.vue'
import HeroSection from '../components/HeroSection.vue'
import ContentSection from '../components/ContentSection.vue'
import PartnersSection from '../components/PartnersSection.vue'
import Footer from '../components/Footer.vue'
</script>

<template>
  <div class="landing-page">
    <Header />
    <HeroSection />
    <ContentSection />
    <PartnersSection />
    <Footer />
  </div>
</template>

<style scoped>
.landing-page {
  display: flex;
  flex-direction: column;
  min-height: 100vh;
}
</style>
