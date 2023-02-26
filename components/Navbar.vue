<template>
    <nav class="bg-white min-w-375 ">
      <div class="container mx-auto px-6 py-4 flex items-center justify-between max-w-screen-xl">
        <div class="w-1/3 flex items-center">
          <img src="https://www.google.com/images/branding/googlelogo/2x/googlelogo_dark_color_272x92dp.png" class="h-8 mr-4" alt="Logo">
        </div>
        <div class="w-1/3 flex items-center ">
          
          
          <div class="flex relative">
            <div class="text-gray-500 ml-5" id="navlist" v-for="menu in navlink" key="menu.name">
              <nuxt-link class="font-poppins" to="{ path: menu.link, query: { itemId: menu.id } }" >
                {{ menu.name }}
          
                <div class="bg-red-500 p-10 font-poppins" v-if="menu.children" v-for="chilrenmenu in menu.children" key="chilerenmenu.text">{{ chilrenmenu.text }}</div>
                
              </nuxt-link>
            </div>

    
          </div>

          
        </div>
        <div class="w-1/3 flex items-center justify-end">
          <nuxt-link class="text-neutral-500 text-lg font-medium mr-4 font-poppins" to="/sign-up">Login</nuxt-link>
          <nuxt-link class="flex justify-start items-center py-4 px-8 font-bold tracking-wide leading-7 rounded-full text-gray-500 border-2 font-poppins" to="/sign-up">Sign Up</nuxt-link>
        </div>
      </div>
    </nav>
  </template>
  
  <script>
    export default {
      data() {
        return {
          navlink:[
          {id:1, name: 'Home',link:"/Home"},
          {id:2, name: "Certificate", link:"/Home", children:[
          {text:"View/Share"},{text:"Tranfer Ownership"}]},
          {id:3, name: "School",link:"/Home"},
          {id:4, name: "How it works",link:"howitworks"},
          {id:5, name: "Contact",link:"/Home"},
          

        ],
          

          
        }
      }
    }
  </script>
  