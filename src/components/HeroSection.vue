<script setup lang="ts">
</script>

<template>
  <section class="hero-section">
    <div class="container">
      <h1 class="hero-title">
        Ecosystem <span class="highlight">Information</span><br />
        <span class="highlight">Point</span> for Amboseli
      </h1>
      
      <p class="hero-subtitle">
        This Ecosystem Information Portal presents narrated, interactive summaries in Maa and Swahili, translating long-term rangeland monitoring data into practical knowledge for communities, partners, and decision-makers across the Amboseli landscape.
      </p>
      
      <button class="btn-primary hero-btn">Open Portal : Hali ya Mazingira – Amboseli Kajiado</button>
    </div>
  </section>
</template>

<style scoped>
.hero-section {
  padding: 5rem 0 3rem;
}

.hero-title {
  font-size: 4.5rem;
  font-weight: 700;
  line-height: 1.1;
  color: var(--color-text-dark);
  margin-bottom: 2rem;
}

.highlight {
  color: var(--color-primary);
}

.hero-subtitle {
  font-size: 1.125rem;
  color: var(--color-text-light);
  max-width: 800px;
  line-height: 1.6;
  margin-bottom: 2.5rem;
}

.hero-btn {
  padding: 1rem 2rem;
  font-size: 1.125rem;
}

@media (max-width: 768px) {
  .hero-title {
    font-size: 3rem;
  }
}
</style>
