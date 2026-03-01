<script setup lang="ts">
</script>

<template>
  <section class="content-section">
    <div class="container">
      <div class="content-grid">
        <div class="image-column">
          <img src="../assets/masai-image.jpg" alt="Maasai woman at server" class="hero-image" />
        </div>
        
        <div class="text-column">
          <h2 class="content-title">Eramatare, Eseriani &<br>Biotisho</h2>
          
          <div class="content-body">
            <p>
              We provide open, practical insights that turn complex monitoring into clear stories about the land, wildlife, and people. By tracking changes in vegetation, rainfall, wildlife, livestock, and settlements, we help communities, researchers, and policymakers anticipate risks, plan better, and take action.
            </p>
            <p>
              We are a collaborative platform, supported by leading conservation partners, that consolidates scientific research and community-sourced data into a single hub. Our mission is to empower local communities, conservancy managers, and government with the evidence needed to make informed decisions that benefit both people and wildlife.
            </p>
          </div>
          
          <button class="btn-primary">Learn More</button>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.content-section {
  padding: 4rem 0;
}

.content-grid {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 4rem;
  align-items: center;
}

.image-column {
  width: 100%;
}

.hero-image {
  width: 100%;
  height: auto;
  border-radius: 4px;
  box-shadow: 0 4px 20px rgba(0, 0, 0, 0.1);
  display: block;
}

.text-column {
  padding-right: 2rem;
}

.content-title {
  font-size: 2.5rem;
  font-weight: 700;
  line-height: 1.2;
  margin-bottom: 2rem;
  color: var(--color-text-dark);
}

.content-body {
  color: var(--color-text-light);
  font-size: 1.05rem;
  margin-bottom: 2.5rem;
}

.content-body p {
  margin-bottom: 1.25rem;
}

@media (max-width: 992px) {
  .content-grid {
    grid-template-columns: 1fr;
    gap: 3rem;
  }
  
  .text-column {
    padding-right: 0;
  }
}
</style>
