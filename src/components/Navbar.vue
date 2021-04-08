<template>
  <nav class="bg-gray-700">
  <div class="max-w-6xl mx-auto px-4">
    <div class="flex justify-between">

      <div class="flex space-x-4">
        <!-- logo -->
        <div>
          <a href="#" class="flex items-center py-5 px-2 text-gray-300 hover:text-gray-400">
            <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 mr-1 text-red-400" viewBox="0 0 20 20" fill="currentColor">
                <path d="M13 7H7v6h6V7z" />
                <path fill-rule="evenodd" d="M7 2a1 1 0 012 0v1h2V2a1 1 0 112 0v1h2a2 2 0 012 2v2h1a1 1 0 110 2h-1v2h1a1 1 0 110 2h-1v2a2 2 0 01-2 2h-2v1a1 1 0 11-2 0v-1H9v1a1 1 0 11-2 0v-1H5a2 2 0 01-2-2v-2H2a1 1 0 110-2h1V9H2a1 1 0 010-2h1V5a2 2 0 012-2h2V2zM5 5h10v10H5V5z" clip-rule="evenodd" />
            </svg>
            <span class="font-bold">ZonyPlay</span>
          </a>
        </div>

        <!-- primary nav -->
        <div class="hidden md:flex items-center space-x-1">
          <a href="#" class="py-5 px-3 text-gray-300 hover:text-gray-400">Tourenments</a>
          <a href="#" class="py-5 px-3 text-gray-300 hover:text-gray-400">LeaderBoard</a>
          <a href="#" class="py-5 px-3 text-gray-300 hover:text-gray-400">Games</a>
        </div>
      </div>

      <!-- secondary nav -->
      <div class="hidden md:flex items-center space-x-1">
        <a href="" class="py-5 px-3 text-gray-300 hover:text-gray-400">Sign In</a>
        <a href="" class="py-2 px-3 bg-red-400 hover:bg-red-300 text-red-900 hover:text-red-800 rounded transition duration-300">Sign Up</a>
      </div>

      <!-- mobile button goes here -->
      <div class="md:hidden flex items-center">
        <button class="mobile-menu-button text-gray-400" v-on:click="desktopView = !desktopView">
          <svg class="w-6 h-6" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16" />
          </svg>
        </button>
      </div>

    </div>
  </div>

  <!-- mobile menu -->
    <div v-if="!desktopView" class="mobile-menu md:hidden">
      <a href="#" class="block py-2 px-4 text-gray-300 hover:text-gray-600 hover:bg-gray-300">Tourenments</a>
      <a href="#" class="block py-2 px-4 text-gray-300 hover:text-gray-600 hover:bg-gray-300">LeaderBoard</a>
      <a href="#" class="block py-2 px-4 text-gray-300 hover:text-gray-600 hover:bg-gray-300">Games</a>
      <a href="#" class="block py-2 px-4 text-gray-300 hover:text-gray-600 hover:bg-gray-300">Sign In</a>
      <a href="#" class="block py-3 px-4 text-red-300 hover:text-red-400 hover:bg-gray-300 ">Sign Up</a>
    </div>
</nav>
</template>

<script>
export default {
  data: () => {
    return{
      desktopView : true,
      showNav : true
    };
    
  },
  methods: {
    
  },
}
</script>

<style>

</style>
