<template>
  <section class="bg-gray-100 min-h-screen  py-12">
    <div class="container mx-auto px-6">
      <h2 class="text-3xl font-bold mb-6">Marketplace</h2>
      <div class="grid grid-cols-1 md:grid-cols-3 lg:grid-cols-4 gap-6">
        <!-- Add marketplace items here -->
        <div class="bg-white p-4 rounded-lg shadow">
          <div class="w-full h-48 bg-gray-200 mb-4 rounded"></div>
          <h3 class="text-lg font-semibold">Item Name</h3>
          <p class="text-gray-600">0.5 ETH</p>
          <button class="mt-4 bg-indigo-600 text-white px-4 py-2 rounded w-full hover:bg-indigo-700 transition duration-300">Buy Now</button>
        </div>
        <!-- Repeat for more items -->
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'Marketplace'
}
</script>