<script setup lang="ts">
import { ref } from 'vue';
import logoAet from '../assets/aet.jpg';
import logoAcp from '../assets/acp.jpg';
import logoLiz from '../assets/liz.jpg';
import logoPolish from '../assets/polish.jpg';
import logoAcc from '../assets/acc.jpg';
import logoEu from '../assets/eu.jpg';
import logoAdac from '../assets/adac.jpg';
import logoMosaic from '../assets/mosaic.jpg';

const partners = ref([
  { id: 1, name: 'Amboseli Ecosystem Trust', src: logoAet },
  { id: 2, name: 'Amboseli Conservation Program', src: logoAcp },
  { id: 3, name: 'Liz Claiborne Art Ortenberg Foundation', src: logoLiz },
  { id: 4, name: 'Polish aid', src: logoPolish },
  { id: 5, name: 'African Conservation Centre', src: logoAcc },
  { id: 6, name: 'European Union', src: logoEu },
  { id: 7, name: 'ADAC', src: logoAdac },
  { id: 8, name: 'Mosaic', src: logoMosaic }
]);
</script>

<template>
  <section class="partners-section">
    <div class="container text-center">
      <h2 class="partners-title">Our Partners</h2>
      <p class="partners-subtitle">
        Our work is powered by our partners and sponsors who invest in monitoring,<br>
        open data, and community engagement across Amboseli.
      </p>
      
      <div class="logos-grid">
        <div v-for="partner in partners" :key="partner.id" class="partner-logo-wrapper">
          <img :src="partner.src" :alt="partner.name" class="partner-logo" />
        </div>
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

.logos-grid {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-wrap: wrap;
  gap: 3rem;
  max-width: 1000px;
  margin: 0 auto;
}

.partner-logo-wrapper {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 80px; 
}

.partner-logo {
  max-width: 200px;
  max-height: 100%;
  object-fit: contain;
}
</style>
