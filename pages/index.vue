<template> 
<!-- max-w-screen-xl -->
<div class="">
<Navbar />
<!-- HeroSection -->
<div class="px-6 mx-auto max-w-screen-xl">
  <div class="flex">
    <div class="pt-24 pr-8 w-1/2">
      <h1 class="text-6xl font-bold font-display">Securely Manage and Verify Your Certificates with NFT</h1>
      <p class="pt-8 max-w-md text-base leading-relaxed text-gray-500">Start managing your certificates securely and transparently with our NFT-based platform</p>
      <div class="flex items-center pt-12 space-x-6">
        <button class="flex justify-center items-center py-4 px-8 font-bold tracking-wide leading-7 text-white bg-orange-600 rounded-full">Sign up</button>
        <button class="flex justify-start items-center py-4 px-8 font-bold tracking-wide leading-7 rounded-full text-gray-500 border-2">Learn More</button>
      </div>
    </div>
    <div class="w-1/2">
      <img src="/ThesisWork.svg" alt="" />
    </div>
  </div>
</div>
<!-- HeroSection -->
<!-- FeatureSection -->
<div class="py-24" id="">
  <div class="w-full max-w-screen-xl mx-auto my-0 px-20 py-0" id="feature-center">
    <div class="max-w-3xl mx-auto my-20 text-center" id="head">
      <p class="text-xs font-bold text-gray-500" id="">EMPOWERING CERTIFICATES</p>
      <h2 class="text-5xl leading-relaxed tracking-tight mb-5 font-bold min-w-375">Building a secure for certificates</h2>
    </div>
    <div class="flex flex-wrap text-left " id="feature-column">
      <div class="w-full md:w-1/3 p-3 py-20 px-8">
        <h4 class="mb-4 font-semibold text-base" id="">Create certificate</h4>
        <p class="text-sm text-gray-500" id="">Each certificate is unique and verifiable on the blockchain, ensuring the authenticity of student achievements.</p>
      </div>
      <div class="w-full md:w-1/3 p-3 border-r border-l py-20 px-8">
        <h4 class="mb-4 font-semibold text-base">Manage Certificate</h4>
        <p class="text-sm text-gray-500" id="">Easily manage all student certificates in one place. Complete control and visibility over the certifications</p>
      </div>
      <div class="w-full md:w-1/3 p-3 py-20 px-8">
        <h4 class="mb-4 font-semibold text-base">View certificate</h4>
        <p class="text-sm text-gray-500" id="">Share your achievements with others and showcase your accomplishments</p>
      </div>
    </div>
  </div>
</div>
<!-- FeatureSection -->
<!-- Benefit section -->
<div class="">
  <div class="relative  bg-gray-100 w-full mx-0 my-auto px-20 py-20" id="benefit-section">
    <div class="" id="benefit-image">
      
    </div>
    <div class="relative z-10 max-w-lg ml-auto p-12 bg-white rounded-3xl shadow-md" id="benefit-wrapper">
      <h2 class="mb-12 text-5xl font-bold">The Benefits of Out Platform</h2>
      <p class="mb-12 text-gray-500">By choosing our platform, students can enjoy a number of benefits including</p>
      <div class="mb-2 " id="benefit-list">

      <!-- Benefit 1 -->
      
        <div v-for="list in benefitlist" key="list.id" class="flex p-6 rounded-xl cursor-pointer hover:border mb-2" id="benefit-item">
          <div  class="flex justify-center shrink-0 w-10 h-10 mr-6" id="benefit-icon">
            <img v-bind:src=" list.img " alt="" />
          </div>
          <div class="grow" id="benefit-details">
            <h5 class="mb-2 font-bold">{{ list.title }}</h5>
            <p class="max-w-xs text-base text-gray-500">{{ list.text }}</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</div>
<!-- Benefit section -->

<Footer />
</div>
</template>

<script>



export default {
  data() {
    return{
      benefitlist:[
        {id:1, img : 'https://www.svgrepo.com/show/74601/security.svg', title:'Security', text: 'abc'},
        {id:2, img : 'https://www.svgrepo.com/show/74601/security.svg', title:'Security', text: 'abc'},
        {id:3, img : 'https://www.svgrepo.com/show/74601/security.svg', title:'Security', text: 'abc'},
        {id:4, img : 'https://www.svgrepo.com/show/74601/security.svg', title:'Security', text: 'abc'},
        {id:5, img : 'https://www.svgrepo.com/show/74601/security.svg', title:'Security', text: 'abc'},
        
      ]
        
    }
}
}



</script>
