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
          
          <router-link to="/portal" class="btn-primary" style="display: inline-block;">Open Portal</router-link>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.content-section {
  padding: 6rem 0;
}

.content-grid {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 5rem;
  align-items: center;
}

.image-column {
  width: 100%;
}

.hero-image {
  width: 100%;
  height: 50vh;
  object-fit: cover; /* This makes it fill the 50vh space without stretching/distorting the aspect ratio */
  display: block;
}

.text-column {
  padding-right: 0;
}

.content-title {
  font-size: 3.25rem;
  font-weight: 700;
  line-height: 1.2;
  margin-bottom: 2rem;
  color: #000000;
}

.content-body {
  color: #000000;
  font-size: 1.1rem;
  margin-bottom: 2.5rem;
}

.content-body p {
  margin-bottom: 1.5rem;
}

@media (max-width: 992px) {
  .content-grid {
    grid-template-columns: 1fr;
    gap: 3rem;
  }
}
</style>
