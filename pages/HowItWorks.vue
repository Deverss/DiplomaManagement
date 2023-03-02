<template>
    
    <div class="max-w-screen-xl min-w-min mx-auto" id="how-it-works">
        <Navbar />
        <div class="" id="how-it-works-center">
            <div class="max-w-lg mb-20" id="how-it-works-header">
                <div class="text-xs mb-3 font-bold text-gray-500 font-poppins" id="stage-small">EXPLORE THE WEB</div>
                <h2 class="mb-5 text-5xl font-bold font-poppins">Protect your certificate</h2>
                <div class="mb-6 text-2xl text-gray-500 font-poppins">Get started with two free weeks of unlimited yoga, fitness, and meditation classes.</div>
                <NuxtLink class="border-2 rounded-3xl px-6 py-3 h-12 items-center text-base font-bold leading-none font-poppins" to="#" id="">Login now</NuxtLink>
            </div>
            <div class="" id="how-it-works-wrap">
                <div class="" id="how-it-works-steps">
                    <div v-for="list in howitworks" key="list.id" class="flex items-center mb-8" id="how-it-works-rows">
                        <div class="pt-8 mx-4 my-0 basis-6/12 w-6/12" id="how-it-works-col">
                            <div class="max-w-xs" id="how-it-works-details">
                                <div class="mb-6 pb-7 text-3xl font-bold border-b-2 font-poppins" id="how-it-works-numbers">{{ list.numbers }}</div>
                                <div class="mb-4 font-bold font-poppins" id="how-it-works-category">{{ list.category }}</div>
                                <div class="text-sm text-gray-500 font-poppins" id="how-it-works-content"> {{ list.content }}</div>
                            </div>
                        </div>
                        <div class="pt-8 mx-4 my-0 basis-6/12 w-6/12" id="how-it-works-col">
                            <div class="" id="how-it-works-preview">
                                <img v-bind:src="list.img" class="w-full rounded-3xl" alt=""/>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        
    <Footer />
    </div>
    
</template>
<script>
export default {
    data() {
      return{
         howitworks: [
            {
                id:1,
                img:'https://images.unsplash.com/photo-1673506073231-3d4896dd45c2?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=2332&q=80',
                numbers:'01.',
                category:'The qwjeijqwiojqw',
                content:'ijfwjeoifjwoiejfiowjefiowjefowejfwoejfoiwejfojweofjw',
            },
            {
                id:2,
                img:'https://images.unsplash.com/photo-1673506073231-3d4896dd45c2?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=2332&q=80',
                numbers:'02.',
                category:'Quickly find the class you want',
                content:'ijfwjeoifjwoiejfiowjefiowjefowejfwoejfoiwejfojweofjw',
            },
            {
                id:3,
                img:'#',
                numbers:'03.',
                category:'jdioasjdoijasoidj',
                content:'ijdiqojd',
            },
            {
                id:4,
                img:'#',
                numbers:'04.',
                category:'jifoejgodifjgojdo',
                content:'ijdiqojd',
            },
         ],
      }
    }
}
</script>