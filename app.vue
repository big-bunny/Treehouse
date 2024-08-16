<template>
  <div class="flex h-screen">
    <nav class="bg-indigo-900 w-20 flex flex-col items-center py-4 space-y-6 shadow-lg">
      <NuxtLink
        v-for="link in links"
        :key="link.name"
        :to="link.to"
        class="relative group flex flex-col items-center p-2 rounded-lg transition-all duration-300 ease-in-out hover:bg-indigo-800"
      >
        <Icon :name="link.icon" class="text-white text-2xl group-hover:text-indigo-200" />
        <span class="absolute left-20 opacity-0 group-hover:opacity-100 transition-opacity duration-300 ease-in-out bg-indigo-800 text-white text-sm px-2 py-1 rounded-md whitespace-nowrap shadow-lg">
          {{ link.name }}
        </span>
      </NuxtLink>

      <button class="bg-white text-indigo-600 px-4 py-2 rounded-full font-semibold hover:bg-indigo-200 transition-all duration-300 ease-in-out shadow-md hover:shadow-lg mt-auto">
        Connect Wallet
      </button>
    </nav>

    <div class="flex-1 overflow-auto bg-gray-100">
      <NuxtPage />
    </div>
  </div>
  
  <footer class="bg-indigo-900 py-4 text-center text-white fixed bottom-0 w-full">
    <div class="container mx-auto">
      <p>&copy; 2024 TREEHOUSE. All rights reserved.</p>
    </div>
  </footer>
</template>

<script setup>
import { ref } from 'vue'

const links = ref([
  { name: 'Home', to: '/', icon: 'mdi:home' },
  { name: 'Explore', to: '/explore', icon: 'mdi:magnify' },
  { name: 'Create', to: '/create', icon: 'mdi:plus-circle' },
  { name: 'MetaBunge', to: '/metabunge', icon: 'mdi:account-group' },
  { name: 'NFT & Crypto', to: '/nft-crypto', icon: 'mdi:currency-btc' },
  { name: 'Marketplace', to: '/marketplace', icon: 'mdi:store' },
  { name: 'Play & Earn', to: '/play-game', icon: 'mdi:gamepad-variant' },
  { name: 'About', to: '/about', icon: 'mdi:information' },
])
</script>

<style>
/* Global styles, if needed */
</style>