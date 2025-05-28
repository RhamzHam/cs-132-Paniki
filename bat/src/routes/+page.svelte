<script>
  // You can import Svelte components or animations here
  import { onMount } from 'svelte';
</script>




<main class="bg-gradient-to-b from-gray-800 via-gray-900 to-black text-gray-100">
  <!-- Hero Section -->
  <div id="top" class="relative h-screen flex items-center justify-center bg-cover bg-center" style="background-image: url('/bat_distribution.png');">
    <div class="absolute inset-0 bg-black bg-opacity-60"></div>
    <div class="relative text-center max-w-2xl px-6">
      <h2 class="text-5xl font-extrabold text-purple-300 mb-4 drop-shadow-lg">Predicting Bat Occurrence<br/>in the Philippine Climate</h2>
      <p class="text-lg mb-6">Analyzing how changing environmental factors impact our native bat populations for better conservation.</p>
      <a href="#overview" class="px-6 py-3 bg-purple-500 hover:bg-purple-600 rounded-full font-semibold">Learn More</a>
    </div>
  </div>

  <!-- Overview -->
  <section id="overview" class="py-20 bg-gray-900">
    <div class="max-w-6xl mx-auto px-6 grid grid-cols-1 md:grid-cols-3 gap-8">
      <div class="text-center p-6 bg-gray-800 rounded-2xl shadow-lg">
        <svg class="mx-auto mb-4 w-12 h-12 text-purple-400" fill="currentColor" viewBox="0 0 16 16"><path d="M8 0C5.878 0 4 1.878 4 4 4 2.895 4.895 2 6 2c.74 0 1.37.402 1.72 1H8v1H6c-2.209 0-4 1.791-4 4v4h2v-4c0-1.103.897-2 2-2h4c1.103 0 2 .897 2 2v4h2v-4c0-2.209-1.791-4-4-4H8V3h.28C9.63 2.402 10.26 2 11 2c1.105 0 2 .895 2 2 0-2.122-1.878-4-4-4z"/></svg>
        <h3 class="text-xl font-semibold mb-2">Motivation</h3>
        <p>Understanding bat populations is crucial for ecosystem health and disease mitigation.</p>
      </div>
      <div class="text-center p-6 bg-gray-800 rounded-2xl shadow-lg">
        <svg class="mx-auto mb-4 w-12 h-12 text-purple-400" fill="currentColor" viewBox="0 0 16 16"><path d="M8 1.5a.5.5 0 01.5.5v1h1a.5.5 0 010 1h-1v1a.5.5 0 01-1 0V4h-1a.5.5 0 010-1h1V2a.5.5 0 01.5-.5z"/><path d="M6 14V6h4v8H6zm6-10h2a2 2 0 012 2v10H2V6a2 2 0 012-2h2v-.5A1.5 1.5 0 016.5 2h3A1.5 1.5 0 0111 3.5V4z"/></svg>
        <h3 class="text-xl font-semibold mb-2">Problem</h3>
        <p>Scarce research on environmental drivers of bat distribution impedes conservation.</p>
      </div>
      <div class="text-center p-6 bg-gray-800 rounded-2xl shadow-lg">
        <svg class="mx-auto mb-4 w-12 h-12 text-purple-400" fill="currentColor" viewBox="0 0 16 16"><path d="M8 0a8 8 0 108 8A8 8 0 008 0zm3.5 9H8v3.5a.5.5 0 01-1 0V9H3.5a.5.5 0 010-1H7V4.5a.5.5 0 011 0V8h3.5a.5.5 0 010 1z"/></svg>
        <h3 class="text-xl font-semibold mb-2">Solution</h3>
        <p>Build species distribution models linking bioclimatic variables to occurrences.</p>
      </div>
    </div>
  </section>

  <!-- Data -->
  <section id="data" class="py-20 bg-gradient-to-b from-gray-900 to-gray-800">
    <div class="max-w-5xl mx-auto px-6">
      <h2 class="text-3xl font-bold text-center mb-8 text-purple-300">Data & Scope</h2>
      <p class="text-center mb-6">We leveraged the BatMapPH dataset (Jan 1, 2000 – May 5, 2024) with 1,739 high-quality occurrences sourced from GBIF and literature repositories.</p>
      <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
        <div class="bg-gray-800 p-6 rounded-2xl shadow-md">
          <h3 class="font-semibold mb-2">Occurrence Records</h3>
          <p>Includes taxonomic and geospatial data cleaned to remove missing species-level entries.</p>
        </div>
        <div class="bg-gray-800 p-6 rounded-2xl shadow-md">
          <h3 class="font-semibold mb-2">Bioclimatic Variables</h3>
          <p>WorldClim SSP585 CMIP6 projections (2021–2040) at 2.5’ resolution for temperature, precipitation, etc.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- Methods -->
  <section id="methods" class="py-20 bg-gray-900">
    <div class="max-w-4xl mx-auto px-6">
      <h2 class="text-3xl font-bold text-center mb-8 text-purple-300">Methods</h2>
      <p class="mb-6">Data preprocessing involved converting GeoTIFF rasters to CSV, spatial joins with occurrence points, and filtering out voids. Linear regression models evaluated temperature and precipitation effects, using R², MSE, and MAE for performance.</p>
      <div class="flex justify-center space-x-8">
        <img src="/world map.png" alt="Spatial preprocessing" class="w-128 rounded-lg shadow-lg" />
        <img src="/linear regression.png" alt="Regression plot" class="w-128 rounded-lg shadow-lg" />
      </div>
    </div>
  </section>

  <!-- Importance -->
  <section id="importance" class="py-20 bg-gradient-to-b from-gray-800 to-gray-900">
    <div class="max-w-3xl mx-auto px-6 text-center">
      <h2 class="text-3xl font-bold mb-4 text-purple-300">Why This Study Matters</h2>
      <p>Bats are vital pollinators, pest controllers, and ecosystem engineers. Understanding how climate change alters their distribution helps inform conservation strategies, disease outbreak prevention, and biodiversity maintenance in the Philippines.</p>
    </div>
  </section>

  <!-- Results -->
  <section id="results" class="py-20 bg-gray-900">
    <div class="max-w-4xl mx-auto px-6">
      <h2 class="text-3xl font-bold text-center mb-6 text-purple-300">Findings</h2>
      <p class="mb-4">Our linear models showed weak individual correlations (e.g., mean annual temperature R² = 0.234), indicating more advanced machine learning methods are needed for accurate prediction.</p>
      <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
        <div class="bg-gray-800 p-6 rounded-lg shadow-md">
          <h3 class="font-semibold mb-2">Temperature Model</h3>
          <p>R² = 0.234, suggesting low explanatory power by itself.</p>
        </div>
        <div class="bg-gray-800 p-6 rounded-lg shadow-md">
          <h3 class="font-semibold mb-2">Future Directions</h3>
          <p>Incorporate random forests, boosted trees, and ensemble learning for improved performance.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- Team & Contact -->
  <section id="team" class="py-20 bg-gray-800">
    <div class="max-w-6xl mx-auto px-6 text-center">
      <h2 class="text-3xl font-bold mb-8 text-purple-300">Meet the Team</h2>
      <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
        <div class="space-y-4">
          <img src="/may.jpg" alt="May Potot" class="mx-auto w-32 h-32 rounded-full shadow-lg" />
          <h3 class="text-xl font-semibold">May Potot</h3>
        </div>
        <div class="space-y-4">
          <img src="/abraham.png" alt="Abraham Sahi" class="mx-auto w-32 h-32 rounded-full shadow-lg" />
          <h3 class="text-xl font-semibold">Abraham Sahi</h3>
        </div>
        <div class="space-y-4">
          <p class="text-lg italic">"Let's hear from you!"</p>
          <a href="mailto:team@batmapph.org" class="text-purple-400 hover:underline">team@batmapph.org</a>
        </div>
      </div>
    </div>
  </section>

  <footer class="py-6 bg-gray-900 text-center text-gray-500">
    &copy; 2025 BatMapPH. All rights reserved.
  </footer>
</main>
