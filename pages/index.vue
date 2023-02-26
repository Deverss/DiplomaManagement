<template> 
<!-- max-w-screen-xl -->
<div class="">
<Navbar />
<!-- HeroSection -->
<div class="px-6 mx-auto max-w-screen-xl">
  <div class="flex">
    <div class="pt-24 pr-8 w-1/2">
      <h1 class="text-6xl font-bold font-displa font-poppins">Your Diplomas, Always Accessible</h1>
      <p class=" pt-8 max-w-md text-base leading-relaxed text-gray-500 font-poppins">Our platform provides a secure and convenient way to store and access all of your university diplomas in one place.</p>
      <div class="flex items-center pt-12 space-x-6">
        <button class="flex justify-center items-center py-4 px-8 font-bold tracking-wide leading-7 text-white bg-orange-600 rounded-full font-poppins">Explore</button>
        <button class="flex justify-start items-center py-4 px-8 font-bold tracking-wide leading-7 rounded-full text-gray-500 border-2 font-poppins">Get started</button>
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
      <p class="text-xs font-bold text-gray-500 font-poppins" id="">EMPOWERING CERTIFICATES</p>
      <h2 class="text-5xl leading-relaxed tracking-tight mb-5 font-bold min-w-375 font-poppins">Building a secure for certificates</h2>
    </div>
    <div class="flex flex-wrap text-left " id="feature-column">
      <div class="w-full md:w-1/3 p-3 py-20 px-8">
        <h4 class="mb-4 font-semibold text-base font-poppins" id="">ICON LOCK Secure Storage</h4>
        <p class="text-sm text-gray-500 font-poppins" id="">Using NFT technology to store and manage your diplomas securely, giving you complete control over your documents.</p>
      </div>
      <div class="w-full md:w-1/3 p-3 border-r border-l py-20 px-8">
        <h4 class="mb-4 font-semibold text-base font-poppins">ICON CLOUD Easy Access</h4>
        <p class="text-sm text-gray-500 font-poppins" id="">Access and share your diplomas from any device with an internet connection, making it easy to stay connected and in control of your documents.</p>
      </div>
      <div class="w-full md:w-1/3 p-3 py-20 px-8">
        <h4 class="mb-4 font-semibold text-base font-poppins">ICON Collaboration Streamlined Collaboration</h4>
        <p class="text-sm text-gray-500 font-poppins" id=""> Easily share and collaborate on your diplomas with others, keeping you organized and in control of your documents.</p>
      </div>
    </div>
  </div>
</div>
<!-- FeatureSection -->
<!-- Benefit section -->
<div class="relative bg-gray-100">
  <div class="relative w-full mx-0 my-auto px-20 py-20 max-w-screen-xl" id="benefit-section">
    <div class="" id="benefit-image">
      
    </div>
    <div class="relative z-10 max-w-lg ml-auto p-12 bg-white rounded-3xl shadow-md" id="benefit-wrapper">
      <h2 class="mb-12 text-5xl font-bold font-poppins">The Benefits of Out Platform</h2>
      <p class="mb-12 text-gray-500 font-poppins">By choosing our platform, students can enjoy a number of benefits including</p>
      <div class="mb-2 " id="benefit-list">

      <!-- Benefit 1 -->
      
        <div v-for="list in benefitlist" key="list.id" class="flex p-6 rounded-xl cursor-pointer hover:border mb-2" id="benefit-item">
          <div  class="flex justify-center shrink-0 w-10 h-10 mr-6" id="benefit-icon">
            <img v-bind:src=" list.img " alt="" />
          </div>
          <div class="grow" id="benefit-details">
            <h5 class="mb-2 font-bold font-poppins">{{ list.title }}</h5>
            <p class="max-w-xs text-base text-gray-500 font-poppins">{{ list.text }}</p>
          </div>
        </div>
        <!-- Benefit 1 -->
      </div>
      
    </div>
  </div>
</div>
<!-- Benefit section -->
<!-- How it works section -->
<div class="px-0 py-36" id="section-step">
  <div class="w-full max-w-lg my-0 mx-auto px-0 py-20" id="step-center">
    <div class="max-w-md text-center mt-0 mx-auto mb-20" id="step-head">
      <h2 class="mb-5 text-5xl font-bold text-center font-poppins">How it works</h2>
      <div class="text-center font-poppins" id="step-info">Stacks is a production-ready library of stackable content blocks built in React Native.</div>
    </div>

    <div class="flex m-0" id="step-list">
      <div v-for="list in howitworkslist" key="list.id" class="relative basis-1/4 w-1/4 mx-4 my-0 text-center" id="step-item">
        <div class="" id="step-icon">
          <img v-bind:src="list.img" alt=""/>
        </div>
        <div class="font-poppins" id="step-number">{{ list.number }}</div>
        <div class="font-poppins" id="step-subtitle">{{ list.subtitle }}</div>
        <div class="font-poppins" id="step-text">{{ list.content }}</div>
      </div>
    </div>
  </div>
</div>
<!-- How it works section -->
<Footer />
</div>
</template>

<script>



export default {
  data() {
    return{
      benefitlist:[
        {id:1, img : 'https://www.svgrepo.com/show/74601/security.svg', title:'Secure Storage', text: 'Keep your diplomas safe from loss or theft with our secure NFT-based technology.'},
        {id:2, img : 'https://www.svgrepo.com/show/74601/security.svg', title:'Complete Control', text: 'Easily access and share your academic records on demand, giving you full control over your information.'},
        {id:3, img : 'https://www.svgrepo.com/show/74601/security.svg', title:'Anywhere Access', text: 'With our platform, you can easily access your diplomas from any device with an internet connection, making it simple to share them with employers, universities, and other organizations.'},
        {id:4, img : 'https://www.svgrepo.com/show/74601/security.svg', title:'Fraud Prevention', text: 'Our NFT-based technology verifies the authenticity of your academic credentials, reducing the risk of fraud or forgery.'},
        {id:5, img : 'https://www.svgrepo.com/show/74601/security.svg', title:'Streamlined Collaboration', text: 'You can easily collaborate with colleagues, mentors, and others in your network by securely sharing your diplomas and other academic records.'},
        
      ],
      howitworkslist:[
        {
          id:1, 
          img:'#',
          number: 'Step 1',
          subtite: 'Receive Your Diploma',
          content: 'Once you graduate from your university or educational institution, you will receive a physical copy of your diploma that includes an NFT.',
        },
        {
          id:2, 
          img:'#',
          number: 'Step 2',
          subtite: 'Access and Share',
          content: 'Your diploma will be securely stored on our platform, and you can easily access and share it with anyone, anywhere in the world.',
        },
        {
          id:3, 
          img:'#',
          number: 'Step 3',
          subtite: 'Verify Authenticity',
          content: 'Employers, universities, and other organizations can quickly and easily verify the authenticity of your academic credentials by checking the blockchain record associated with your NFT.',
        },
        {
          id:4, 
          img:'#',
          number: 'Step 4',
          subtite: 'Manage Your Records',
          content: 'With our platform, you can easily manage all of your academic records in one place, streamlining the application process and simplifying your life.',
        },
      ]
        
    }
}
}



</script>
