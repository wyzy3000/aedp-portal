<script setup lang="ts">
</script>

<template>
  <section class="partners-section">
    <div class="container text-center">
      <h2 class="partners-title">Our Partners</h2>
      <p class="partners-subtitle">
        Our work is powered by our partners and sponsors who invest in monitoring,<br>
        open data, and community engagement across Amboseli.
      </p>
      
      <div class="logos-container">
        <img src="../assets/partner-logos.png" alt="Partner Logos" class="partner-logos" />
      </div>
    </div>
  </section>
</template>

<style scoped>
.partners-section {
  padding: 5rem 0;
}

.text-center {
  text-align: center;
}

.partners-title {
  font-size: 2.5rem;
  font-weight: 700;
  margin-bottom: 1.5rem;
  color: var(--color-text-dark);
}

.partners-subtitle {
  font-size: 1.125rem;
  color: var(--color-text-light);
  line-height: 1.6;
  margin-bottom: 4rem;
}

.logos-container {
  max-width: 1000px;
  margin: 0 auto;
}

.partner-logos {
  width: 100%;
  height: auto;
  display: block;
}
</style>
