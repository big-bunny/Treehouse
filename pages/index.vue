<script setup lang="ts">
const route = useRoute()
</script>

<template>
  <div class="min-h-screen bg-gradient-to-br from-indigo-600 to-purple-700 text-white">
    <!-- Hero Section -->
    <header class="container mx-auto px-6 py-16 text-center">
      <h1 class="text-5xl md:text-6xl font-bold mb-6">Welcome to TREEHOUSE</h1>
      <p class="text-xl md:text-2xl mb-8">The decentralized video platform for creators and viewers</p>
      <NuxtLink 
        to="/explore" 
        class="bg-white text-indigo-600 px-8 py-3 rounded-full font-semibold text-lg hover:bg-indigo-100 transition"
      >
        Explore Videos
      </NuxtLink>
    </header>

    <!-- Features Section -->
    <section class="container mx-auto px-6 py-16">
      <h2 class="text-3xl font-bold text-center mb-12">Why Choose TREEHOUSE?</h2>
      <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
        <div class="bg-white bg-opacity-10 p-6 rounded-lg">
          <h3 class="text-xl font-semibold mb-4">Decentralized Storage</h3>
          <p>Your content stays yours, stored securely on the blockchain.</p>
        </div>
        <div class="bg-white bg-opacity-10 p-6 rounded-lg">
          <h3 class="text-xl font-semibold mb-4">Fair Monetization</h3>
          <p>Earn cryptocurrency directly from your viewers, no middlemen.</p>
        </div>
        <div class="bg-white bg-opacity-10 p-6 rounded-lg">
          <h3 class="text-xl font-semibold mb-4">Censorship Resistant</h3>
          <p>Express yourself freely without fear of arbitrary takedowns.</p>
        </div>
      </div>
    </section>

    <!-- CTA Section -->
    <section class="container mx-auto px-6 py-16 text-center">
      <h2 class="text-3xl font-bold mb-6">Ready to Join the Revolution?</h2>
      <p class="text-xl mb-8">Start uploading your videos and connecting with your audience today.</p>
      <a href="#" class="bg-white text-indigo-600 px-8 py-3 rounded-full font-semibold text-lg hover:bg-indigo-100 transition">
        Create Your Channel
      </a>
    </section>

    <!-- Debug Information (you can remove this in production) -->
    <div class="container mx-auto px-6 py-8 text-center">
      <p class="text-lg">Current route: {{ route.path }}</p>
      <a href="https://nuxt.com/docs/getting-started/routing" target="_blank" class="text-indigo-300 hover:text-indigo-100">Learn more about Nuxt Routing</a>
    </div>
  </div>
</template>
<style>

</style>