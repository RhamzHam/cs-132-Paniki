<script>
  // You can import Svelte components or animations here
  import { onMount } from 'svelte';
</script>




<main class="bg-gradient-to-b from-gray-800 via-gray-900 to-black text-gray-100">
  <!-- Hero Section -->
  <div id="top" class="relative h-screen flex items-center justify-center bg-cover bg-center" style="background-image: url('/bat_distribution.png');">
    <div class="absolute inset-0 bg-black bg-opacity-60"></div>
    <div class="relative text-center max-w-2xl px-6 text-white">
        <h2 class="text-5xl font-extrabold text-purple-300 mb-4 drop-shadow-lg">Predicting Bat Occurrence<br/>in the Philippine Climate</h2>
        <p class="text-lg mb-6">Analyzing how changing environmental factors impact our native bat populations for better conservation.</p>

        <!-- Project Description -->
        <p class="mb-4">
        And this is our project, <strong>Analyzing the Relationship Between Environmental Factors and Bat Population in the Philippines</strong>.
        This project aims to analyze the correlation of different environmental factors such as climate, humidity, wildlife, etc. to the population of bats in the Philippines.
        It also aims to highlight the bat species that are most endangered due to changing climate conditions.
        </p>

        <!-- Team Members -->
        <p class="font-semibold">Data Science Team</p>
        <ul class="mt-2 space-y-1">
        <li>May Potot, WFX Autumn</li>
        <li>Abraham Sahi, WFX Autumn</li>
        </ul>
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

  <div id="top" class="relative h-screen flex items-center justify-center" style="background-image: url('https://images.squarespace-cdn.com/content/v1/545b3746e4b0a4696b72a563/1591949371083-N6C2EPMKH05UWM8ZIUOF/shutterstock_1282913071.jpg?format=1500w');">
    <div class="absolute inset-0 bg-black bg-opacity-60"></div>
    <div class="relative text-center max-w-3xl px-6">
        <h2 class="text-5xl font-extrabold text-purple-300 mb-4 drop-shadow-lg">
        Importance of Bat Conservation in the Philippines
        </h2>
        <p class="text-lg mb-6 text-white">
        Bats are critical to the ecological balance of the Philippines, functioning as natural pest regulators, pollinators, and seed dispersers. Despite their importance, bat populations across the country are under growing threat due to rapid environmental changes brought by climate change, deforestation, and urban development. These factors lead to habitat fragmentation and make it harder for researchers and conservationists to predict where bat species are likely to occur. This project addresses that gap by analyzing environmental and climate data to model the occurrence of native bat species across the archipelago. Through this work, we aim to empower conservation efforts with data-driven insights, enabling more strategic habitat protection and resource allocation to preserve the country's unique biodiversity.
        </p>
    </div>
    </div>

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
<!-- Methodology Section -->
<section id="methodology" class="bg-gray-900 text-white py-20 px-6">
  <div class="max-w-4xl mx-auto text-center">
    <h2 class="text-4xl font-extrabold text-purple-300 mb-6 drop-shadow">Our Data Science Methodology</h2>
    <p class="text-lg leading-relaxed text-gray-300">
      In order to identify which environmental factors influence bat populations, we compared our occurrence data to WorldClim’s bioclimatic variables. Specifically, we used the ssp585 CMIP6 downscaled future climate projections (2021–2040) at a resolution of 2.5 arc minutes and sought statistical correlations with BatMapPh’s bat occurrence dataset.
    </p>
    <p class="text-lg leading-relaxed text-gray-300 mt-4">
      Linear regression was our primary method to evaluate the relationship between environmental factors and bat presence. We began with essential data cleaning—removing NaN values and filtering relevant columns to maintain data accuracy. Our key predictors included temperature and precipitation, chosen as the main independent variables, while bat occurrence data served as the dependent variable.
    </p>
    <p class="text-lg leading-relaxed text-gray-300 mt-4">
      With our dataset split into training and testing sets, we trained the regression model to understand the linear relationship. Model performance was evaluated using R², Mean Squared Error (MSE), and Mean Absolute Error (MAE). This structured approach provided a strong foundation for assessing the influence of climate on bat populations, and it opens pathways for including more complex variables in future research.
    </p>
    <div class="flex flex-row justify-center mt-8 space-x-4 p-4">
        <img src="/world map.png" alt="Spatial preprocessing" class="w-128 rounded-lg shadow-lg" />
        <img src="/linear regression.png" alt="Regression plot" class="w-128 rounded-lg shadow-lg" />

    </div>
  </div>

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
