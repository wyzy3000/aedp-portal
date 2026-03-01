<script setup lang="ts">
</script>

<template>
  <div class="portal-layout">
    <!-- Top Header -->
    <header class="portal-header">
      <div class="header-left">
        <h1>Ecosystem Information Point for Kajiado County in Local Languages (Biostisho)</h1>
        <button class="menu-btn" aria-label="Toggle Menu">
          <svg viewBox="0 0 24 24" width="24" height="24" stroke="currentColor" stroke-width="2" fill="none" stroke-linecap="round" stroke-linejoin="round" class="css-i6dzq1"><line x1="3" y1="12" x2="21" y2="12"></line><line x1="3" y1="6" x2="21" y2="6"></line><line x1="3" y1="18" x2="21" y2="18"></line></svg>
        </button>
      </div>
      <div class="header-right">
        <!-- Placeholder for header images if needed -->
        <router-link to="/" class="back-link">Back to Home</router-link>
      </div>
    </header>

    <div class="portal-body">
      <!-- Sidebar -->
      <aside class="sidebar">
        <nav class="sidebar-nav">
          <a href="#" class="nav-item active">
            <span class="icon">🌱</span>
            Pasture (grass) level (Kiwango cha Nyasi)
          </a>
          <a href="#" class="nav-item">
            <span class="icon">🌲</span>
            Amboseli Habitat Changes from aerial monitoring (Hali ya miti)
          </a>
          <a href="#" class="nav-item">
            <span class="icon">📔</span>
            Community Environmental Diaries (Maoni ya wenyeji)
          </a>
          <a href="#" class="nav-item">
            <span class="icon">☁️</span>
            Realtime Weather Forecast (Hali ya anga)
          </a>
          <a href="#" class="nav-item">
            <span class="icon">📊</span>
            Amboseli Outlook Reports (Taarifa za Amboseli)
          </a>
          <a href="#" class="nav-item">
            <span class="icon">📡</span>
            The Satellite Drought Story (2022-2023)
          </a>
          <a href="#" class="nav-item">
            <span class="icon">🩺</span>
            One-Health & Wellbeing (Biotisho, Eseriani, Eramatare)
          </a>
          <a href="#" class="nav-item">
            <span class="icon">ℹ️</span>
            About this Ecosystem Information Point
          </a>
        </nav>
      </aside>

      <!-- Main Content -->
      <main class="main-content">
        <div class="content-card">
          <div class="card-header">
            <h2>The grass story of Amboseli over the years</h2>
          </div>
          
          <div class="card-body">
            <h3 class="chart-title">Amboseli's Pasture (grass) Barometer</h3>
            
            <div class="chart-container">
              <!-- Placeholder for the actual interactive chart -->
              <div class="chart-placeholder">
                <div class="band band-good">Good</div>
                <div class="band band-average">Average</div>
                <div class="band band-poor">Poor</div>
                <div class="mock-line"></div>
                <div class="y-axis">Biomass. g/m²</div>
                <div class="x-axis">Time</div>
              </div>
            </div>

            <div class="action-buttons">
              <button class="btn-play">
                <span class="icon">🔊</span> Play Explanation (Maa language)
              </button>
              <button class="btn-stop">
                <span class="icon">⏹️</span> Stop
              </button>
            </div>
          </div>
        </div>
      </main>
    </div>
  </div>
</template>

<style scoped>
.portal-layout {
  display: flex;
  flex-direction: column;
  height: 100vh;
  background-color: #f0f4f8; /* Light gray background for the app */
  font-family: 'Inter', sans-serif;
}

/* Header */
.portal-header {
  background-color: #3182CE; /* Vibrant Blue */
  color: white;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 0;
  height: 60px;
  box-shadow: 0 2px 4px rgba(0,0,0,0.1);
  z-index: 10;
}

.header-left {
  display: flex;
  align-items: center;
  height: 100%;
}

.header-left h1 {
  font-size: 1.1rem;
  font-weight: 600;
  padding: 0 1.5rem;
  margin: 0;
  background-color: rgba(0,0,0,0.1);
  height: 100%;
  display: flex;
  align-items: center;
}

.menu-btn {
  background: transparent;
  border: none;
  color: white;
  padding: 0 1.5rem;
  cursor: pointer;
  display: flex;
  align-items: center;
}

.header-right {
  padding-right: 1.5rem;
}

.back-link {
  color: white;
  text-decoration: none;
  font-size: 0.9rem;
  font-weight: 500;
  padding: 0.5rem 1rem;
  border: 1px solid rgba(255,255,255,0.3);
  border-radius: 4px;
  transition: background-color 0.2s;
}

.back-link:hover {
  background-color: rgba(255,255,255,0.1);
}

/* Body layout */
.portal-body {
  display: flex;
  flex: 1;
  overflow: hidden;
}

/* Sidebar */
.sidebar {
  width: 320px;
  background-color: #2D3748; /* Dark slate */
  color: #A0AEC0;
  display: flex;
  flex-direction: column;
  overflow-y: auto;
}

.sidebar-nav {
  padding: 1rem 0;
  display: flex;
  flex-direction: column;
}

.nav-item {
  display: flex;
  align-items: center;
  padding: 1rem 1.5rem;
  color: #E2E8F0;
  text-decoration: none;
  font-size: 0.95rem;
  border-left: 4px solid transparent;
  transition: all 0.2s ease;
  line-height: 1.4;
}

.nav-item:hover {
  background-color: rgba(255,255,255,0.05);
  color: white;
}

.nav-item.active {
  background-color: rgba(0,0,0,0.2);
  border-left-color: #4299E1; /* Light blue accent */
  color: white;
}

.nav-item .icon {
  margin-right: 1rem;
  font-size: 1.2rem;
  width: 24px;
  text-align: center;
  opacity: 0.8;
}

/* Main Content */
.main-content {
  flex: 1;
  padding: 2rem;
  overflow-y: auto;
  display: flex;
  justify-content: center;
}

.content-card {
  background: white;
  width: 100%;
  max-width: 1200px;
  border-radius: 4px;
  box-shadow: 0 1px 3px rgba(0,0,0,0.1);
  overflow: hidden;
  border: 1px solid #E2E8F0;
  display: flex;
  flex-direction: column;
}

.card-header {
  background-color: #4299E1; /* Secondary blue */
  color: white;
  padding: 1rem 1.5rem;
}

.card-header h2 {
  font-size: 1.1rem;
  font-weight: 500;
  margin: 0;
}

.card-body {
  padding: 2rem;
  display: flex;
  flex-direction: column;
  align-items: center;
}

.chart-title {
  color: #1A202C;
  font-size: 1.5rem;
  font-weight: 700;
  margin-bottom: 2rem;
  text-align: center;
}

/* Chart Placeholder CSS */
.chart-container {
  width: 100%;
  max-width: 900px;
  margin-bottom: 2rem;
}

.chart-placeholder {
  position: relative;
  height: 400px;
  border-left: 1px solid #CBD5E0;
  border-bottom: 1px solid #CBD5E0;
  padding-left: 1rem;
  padding-bottom: 1rem;
  display: flex;
  flex-direction: column-reverse;
}

.band {
  width: 100%;
  padding: 1rem;
  color: white;
  font-weight: bold;
  font-size: 0.9rem;
  opacity: 0.4;
  display: flex;
  justify-content: center;
  align-items: center;
  text-transform: uppercase;
  letter-spacing: 1px;
}

.band-poor { background-color: #F56565; height: 25%; }
.band-average { background-color: #ED8936; height: 35%; }
.band-good { background-color: #48BB78; height: 40%; }

.mock-line {
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background-image: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 100 100" preserveAspectRatio="none"><polyline fill="none" stroke="gray" stroke-width="0.5" stroke-dasharray="2,2" points="0,80 10,70 20,90 30,50 40,85 50,40 60,60 70,20 80,70 90,30 100,60" /></svg>');
  background-size: 100% 100%;
  opacity: 0.7;
  pointer-events: none;
}

.y-axis {
  position: absolute;
  left: -40px;
  top: 50%;
  transform: translateY(-50%) rotate(-90deg);
  color: #718096;
  font-size: 0.85rem;
}

.x-axis {
  position: absolute;
  bottom: -30px;
  left: 50%;
  transform: translateX(-50%);
  color: #718096;
  font-size: 0.85rem;
}

/* Action Buttons */
.action-buttons {
  display: flex;
  gap: 1rem;
  width: 100%;
  max-width: 900px;
  justify-content: flex-start;
}

.action-buttons button {
  display: flex;
  align-items: center;
  padding: 0.75rem 1.5rem;
  border-radius: 4px;
  font-weight: 600;
  font-size: 0.95rem;
  transition: filter 0.2s;
}

.action-buttons button:hover {
  filter: brightness(0.9);
}

.action-buttons .icon {
  margin-right: 0.5rem;
}

.btn-play {
  background-color: #38A169; /* Green */
  color: white;
}

.btn-stop {
  background-color: #E53E3E; /* Red */
  color: white;
}

@media (max-width: 1024px) {
  .portal-body {
    flex-direction: column;
  }
  .sidebar {
    width: 100%;
    height: auto;
    max-height: 250px;
  }
  .header-left h1 {
    font-size: 0.9rem;
  }
}
</style>
