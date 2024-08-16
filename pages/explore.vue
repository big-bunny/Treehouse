<template>
    <div class="min-h-screen bg-gray-900 text-white">
      <NuxtRouteAnnouncer />
 
  
      <!-- Main Content -->
      <main class="container mx-auto px-6 py-8">
        <h1 class="text-4xl font-bold mb-8 text-center">
          Explore the <span class="text-indigo-400">Treehouse</span> Universe
        </h1>
  
        <!-- Search Bar -->
        <div class="mb-12">
          <div class="relative">
            <input 
              type="text" 
              placeholder="Search for videos, creators, or tags"
              class="w-full bg-gray-800 border-2 border-indigo-500 rounded-full py-3 px-6 pl-12 focus:outline-none focus:border-indigo-400"
            >
            <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 absolute left-4 top-3.5 text-gray-400" fill="none" viewBox="0 0 24 24" stroke="currentColor">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M21 21l-6-6m2-5a7 7 0 11-14 0 7 7 0 0114 0z" />
            </svg>
          </div>
        </div>
  
        <!-- Categories -->
        <section class="mb-16">
          <h2 class="text-2xl font-semibold mb-6">Trending Categories</h2>
          <div class="grid grid-cols-2 md:grid-cols-4 gap-4">
            <div v-for="category in ['Anguka Nayo','Gaming', 'Music', 'Art', 'Tech', 'Travel', 'Sports', 'Education', 'Crypto']" 
                 :key="category"
                 class="bg-gradient-to-br from-indigo-600 to-purple-600 rounded-lg p-6 text-center hover:from-indigo-500 hover:to-purple-500 transition duration-300 cursor-pointer">
              <p class="font-semibold text-lg">{{ category }}</p>
            </div>
          </div>
        </section>
  
        <!-- Trending Videos -->
        <section class="mb-16">
          <h2 class="text-2xl font-semibold mb-6">Trending Videos</h2>
          <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
            <div v-for="i in 6" :key="i" class="bg-gray-800 rounded-lg overflow-hidden hover:shadow-lg transition duration-300">
              <div class="aspect-w-16 aspect-h-9 bg-gray-700"></div>
              <div class="p-4">
                <h3 class="font-semibold text-lg mb-2">Awesome Video Title</h3>
                <p class="text-gray-400 text-sm mb-2">Creator Name</p>
                <div class="flex justify-between text-sm text-gray-500">
                  <span>1.2M views</span>
                  <span>2 days ago</span>
                </div>
              </div>
            </div>
          </div>
        </section>
  
        <!-- Live Now -->
        <section>
          <h2 class="text-2xl font-semibold mb-6">Live Now</h2>
          <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
            <div v-for="i in 3" :key="i" class="bg-gray-800 rounded-lg overflow-hidden hover:shadow-lg transition duration-300 border border-red-500">
              <div class="aspect-w-16 aspect-h-9 bg-gray-700 relative">
                <span class="absolute top-2 left-2 bg-red-500 text-white px-2 py-1 rounded-full text-xs font-semibold">LIVE</span>
              </div>
              <div class="p-4">
                <h3 class="font-semibold text-lg mb-2">Live Stream Title</h3>
                <p class="text-gray-400 text-sm mb-2">Streamer Name</p>
                <div class="flex justify-between text-sm text-gray-500">
                  <span>10.5K watching</span>
                  <span>Started 2h ago</span>
                </div>
              </div>
            </div>
          </div>
        </section>
      </main>
  
   
    </div>
  </template>