<template>
  <section class="bg-gradient-to-br min-h-screen from-indigo-900 to-purple-800 py-16 text-white">
    <div class="container mx-auto px-6">
      <h2 class="text-4xl font-bold mb-8 text-center">MetaBunge: Virtual Assembly</h2>
      <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
        <div class="bg-white bg-opacity-10 p-8 rounded-lg shadow-lg backdrop-filter backdrop-blur-lg hover:bg-opacity-20 transition duration-300">
          <h3 class="text-2xl font-semibold mb-4">Holo-Chamber Debate</h3>
          <p class="mb-4">Immerse yourself in live parliamentary discussions in our virtual reality chamber.</p>
          <button class="bg-indigo-600 text-white px-6 py-3 rounded-full hover:bg-indigo-700 transition duration-300">Enter VR Session</button>
        </div>
        <div class="bg-white bg-opacity-10 p-8 rounded-lg shadow-lg backdrop-filter backdrop-blur-lg hover:bg-opacity-20 transition duration-300">
          <h3 class="text-2xl font-semibold mb-4">Quantum Whisper Pod</h3>
          <p class="mb-4">Tune into our encrypted audio streams for real-time policy discussions.</p>
          <button class="bg-indigo-600 text-white px-6 py-3 rounded-full hover:bg-indigo-700 transition duration-300">Stream Now</button>
        </div>
        <div class="bg-white bg-opacity-10 p-8 rounded-lg shadow-lg backdrop-filter backdrop-blur-lg hover:bg-opacity-20 transition duration-300">
          <h3 class="text-2xl font-semibold mb-4">Nexus Forum</h3>
          <p class="mb-4">Engage in threaded discussions on pressing issues and proposed legislation.</p>
          <button class="bg-indigo-600 text-white px-6 py-3 rounded-full hover:bg-indigo-700 transition duration-300">Join Discourse</button>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'MetaBunge'
}
</script>