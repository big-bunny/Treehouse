<template>
    <div class="relative group">
      <button class="text-white hover:text-indigo-200 transition">eBunge</button>
      <div class="absolute right-0 mt-2 w-48 bg-white rounded-md shadow-lg py-1 z-10 hidden group-hover:block">
        <a v-for="session in activeSessions" :key="session.id" :href="session.link" class="block px-4 py-2 text-sm text-gray-700 hover:bg-indigo-100">
          {{ session.name }}
        </a>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'EBungeDropdown',
    data() {
      return {
        activeSessions: [
          { id: 1, name: 'Climate Policy Debate', link: '#' },
          { id: 2, name: 'Education Reform Pod', link: '#' },
          { id: 3, name: 'Economic Strategy Forum', link: '#' },
        ]
      }
    }
  }
  </script>