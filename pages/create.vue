<template>
    <div class="min-h-screen bg-gray-900 text-white">
      <main class="container mx-auto px-6 py-12">
        <h1 class="text-4xl font-bold mb-8 text-center">
          Create on <span class="text-indigo-400">Treehouse</span>
        </h1>
  
        <div class="grid md:grid-cols-2 gap-12">
          <!-- Upload Video Section -->
          <div class="bg-gray-800 rounded-lg p-8">
            <h2 class="text-2xl font-semibold mb-6">Upload a Video</h2>
            <form @submit.prevent="uploadVideo">
              <div class="mb-4">
                <label for="title" class="block mb-2">Title</label>
                <input type="text" id="title" v-model="videoTitle" class="w-full bg-gray-700 rounded px-3 py-2">
              </div>
              <div class="mb-4">
                <label for="description" class="block mb-2">Description</label>
                <textarea id="description" v-model="videoDescription" rows="4" class="w-full bg-gray-700 rounded px-3 py-2"></textarea>
              </div>
              <div class="mb-6">
                <label for="video" class="block mb-2">Video File</label>
                <input type="file" id="video" accept="video/*" class="w-full bg-gray-700 rounded px-3 py-2">
              </div>
              <button type="submit" class="bg-indigo-600 hover:bg-indigo-700 px-6 py-2 rounded-full transition duration-300">
                Upload Video
              </button>
            </form>
          </div>
  
          <!-- Start Live Stream Section -->
          <div class="bg-gray-800 rounded-lg p-8">
            <h2 class="text-2xl font-semibold mb-6">Start a Live Stream</h2>
            <form @submit.prevent="startLiveStream">
              <div class="mb-4">
                <label for="streamTitle" class="block mb-2">Stream Title</label>
                <input type="text" id="streamTitle" v-model="streamTitle" class="w-full bg-gray-700 rounded px-3 py-2">
              </div>
              <div class="mb-6">
                <label for="category" class="block mb-2">Category</label>
                <select id="category" v-model="streamCategory" class="w-full bg-gray-700 rounded px-3 py-2">
                  <option value="gaming">Gaming</option>
                  <option value="music">Music</option>
                  <option value="talk-show">Talk Show</option>
                  <option value="education">Education</option>
                </select>
              </div>
              <button type="submit" class="bg-red-600 hover:bg-red-700 px-6 py-2 rounded-full transition duration-300">
                Go Live
              </button>
            </form>
          </div>
        </div>
      </main>
    </div>
  </template>
  
  <script setup lang="ts">
  const videoTitle = ref('')
  const videoDescription = ref('')
  const streamTitle = ref('')
  const streamCategory = ref('gaming')
  
  const uploadVideo = () => {
    // Implement video upload logic
    console.log('Uploading video:', videoTitle.value, videoDescription.value)
  }
  
  const startLiveStream = () => {
    // Implement live stream start logic
    console.log('Starting live stream:', streamTitle.value, streamCategory.value)
  }
  </script>