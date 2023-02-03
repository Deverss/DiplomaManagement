<template>
    <nav class="bg-white min-w-375 ">
      <div class="container mx-auto px-6 py-4 flex items-center justify-between max-w-screen-xl">
        <div class="w-1/3 flex items-center">
          <img src="https://www.google.com/images/branding/googlelogo/2x/googlelogo_dark_color_272x92dp.png" class="h-8 mr-4" alt="Logo">
        </div>
        <div class="w-2/3 flex items-center">
          <nuxt-link class="text-neutral-500 text-lg font-medium mr-4" to="/">Home</nuxt-link>
          
          <div class="relative">
            <button class="text-neutral-500 text-lg font-medium mr-4" @mouseover="toggleDropdown" @mouseleave="toggleDropdown" @click="toggleDropdown" to="/certificates">Certificates</button>
            <div class="absolute right-0 py-2 w-48 bg-gray-800 rounded-md shadow-md" v-if="showDropdown">
              <nuxt-link class="block px-4 py-2 text-gray-100 hover:bg-gray-900" to="/schools/mint-nfts">View / Share</nuxt-link>
              <nuxt-link class="block px-4 py-2 text-gray-100 hover:bg-gray-900" to="/schools/verify-authenticity">Transfer Ownership</nuxt-link>
            </div>
          </div>

          <div class="relative">
            <button class="text-neutral-500 font-medium mr-4" @mouseover="toggleDropdown" @mouseleave="toggleDropdown" @click="toggleDropdown">Schools</button>
            <div class="absolute right-0 py-2 w-48 bg-gray-800 rounded-md shadow-md" v-if="showDropdown">
              <nuxt-link class="block px-4 py-2 text-neutral-500 hover:bg-gray-900" to="/schools/mint-nfts">Mint NFTs</nuxt-link>
              <nuxt-link class="block px-4 py-2 text-neutral-500 hover:bg-gray-900" to="/schools/verify-authenticity">Verify Authenticity</nuxt-link>
            </div>
          </div>
          <nuxt-link class="text-neutral-500 text-lg font-medium mr-4" to="/how-it-works">How it Works</nuxt-link>
          <nuxt-link class="text-neutral-500 text-lg font-medium mr-4" to="/contact">Contact</nuxt-link>
          <nuxt-link class="text-neutral-500 text-lg font-medium mr-4" to="/privacy-policy">Privacy Policy</nuxt-link>
        </div>
        <div class="w-1/3 flex items-center justify-end">
          <nuxt-link class="text-neutral-500 text-lg font-medium mr-4" to="/sign-up">Login</nuxt-link>
          <nuxt-link class="flex justify-start items-center py-4 px-8 font-bold tracking-wide leading-7 rounded-full text-gray-500 border-2" to="/sign-up">Sign Up</nuxt-link>
        </div>
      </div>
    </nav>
  </template>
  
  <script>
  export default {
    data() {
      return {
        showDropdown: false
      }
    },
    methods: {
      toggleDropdown() {
        this.showDropdown = !this.showDropdown
      }
      
    }
  }
  </script>
  