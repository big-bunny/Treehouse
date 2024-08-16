<template>
    <div class="bg-gradient-to-r from-purple-500 to-indigo-600 min-h-screen py-12 px-4 sm:px-6 lg:px-8">
      <div class="max-w-7xl mx-auto">
        <h1 class="text-4xl font-extrabold text-white text-center mb-8">Play & Earn Crypto</h1>
        
        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
          <!-- Game Card -->
          <div v-for="game in games" :key="game.id" class="bg-white rounded-lg shadow-xl overflow-hidden">
            <div class="h-48 bg-gray-200 flex items-center justify-center">
              <span class="text-4xl">🎮</span>
            </div>
            <div class="p-6">
              <h3 class="text-xl font-semibold text-gray-900 mb-2">{{ game.name }}</h3>
              <p class="text-gray-600 mb-4">{{ game.description }}</p>
              <div class="flex justify-between items-center">
                <span class="text-indigo-600 font-bold">Reward: {{ game.reward }}</span>
                <button @click="playGame(game.id)" class="bg-indigo-600 text-white px-4 py-2 rounded-full hover:bg-indigo-700 transition duration-300">
                  Play Now
                </button>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'PlayGame',
    data() {
      return {
        games: [
          { id: 1, name: 'Crypto Crusher', description: 'Match 3 crypto symbols to earn tokens!', reward: '0.01 ETH' },
          { id: 2, name: 'Ng`anya-chain', description: 'Race against time to solve blockchain puzzles!', reward: '5 TREE' },
          { id: 3, name: 'NFT Collector', description: 'Collect rare NFTs and build your virtual gallery!', reward: '1 NFT' },
          { id: 4, name: 'DeFi Defender', description: 'Protect your assets from crypto villains!', reward: '0.1 BNB' },
          { id: 5, name: 'Metaverse Miner', description: 'Mine virtual resources in the metaverse!', reward: '50 SAND' },
          { id: 6, name: 'Token Trader', description: 'Test your trading skills in a simulated market!', reward: '100 USDT' },
        ]
      }
    },
    methods: {
      playGame(gameId) {
        // Here you would implement the logic to start the game
        // For now, we'll just log a message
        console.log(`Starting game ${gameId}`)
        // You could also navigate to a specific game page:
        // this.$router.push(`/game/${gameId}`)
      }
    }
  }
  </script>