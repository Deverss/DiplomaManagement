<template>
    <div class="border-t" id="footer">
        <div class="" id="footer-body">
            <div class="flex justify-center w-full max-w-screen-xl mx-auto my-0  py-0" id="footer-center">
                <div class="flex pl-0 py-20 px-20" id="footer-col">
                    <div class="flex flex-col items-start mr-24" id="footer-box">
                        <img src="https://www.google.com/images/branding/googlelogo/2x/googlelogo_dark_color_272x92dp.png" class="h-8 mr-4" alt="Logo">
                    </div>

                    <div class="" id="footer-item">
                        <div class="flex flex-col items-start " id="footer-menu">
                            <NuxtLink class="mb-3.5 text-sm font-bold text-gray-600 font-poppins" to="contact">Our team</NuxtLink>
                            <NuxtLink class="mb-3.5 text-sm font-bold text-gray-600 font-poppins" to="certificates">Certificates</NuxtLink>
                            <NuxtLink class="mb-3.5 text-sm font-bold text-gray-600 font-poppins" to="howitworks">How it Works</NuxtLink>
                            <NuxtLink class="mb-3.5 text-sm font-bold text-gray-600 font-poppins" to="privacy">Privacy Policy</NuxtLink>
                            <NuxtLink class="mb-3.5 text-sm font-bold text-gray-600 font-poppins" to="term">Terms of Service</NuxtLink>
                        </div>
                    </div>
                </div>
                <div class="flex py-20 px-20 border-l" id="footer-col">
                    <div class="" id="footer-item">
                        <div class="mb-10 text-xs leading-none font-bold uppercase" id="footer-category">Contact</div>
                        <div class="text-sm" id="footer-info">
                            <p class="pb-2 font-poppins">188 Quach Thi Trang</p>
                            <p class="pb-2 font-poppins">Hoa Xuan, Cam Le</p>
                            <p class="pb-2 font-poppins">Da Nang</p>
                            <p class="pb-2 font-poppins">0924 603 808</p>
                        </div>
                    </div>
                </div>
                <div class="flex r-0 py-20 pl-20 border-l" id="footer-col">
                    <div class="" id="footer-item">
                        <div class="mb-10 text-xs leading-none font-bold uppercase" id="footer-category">NEWSLETTER</div>
                        <div class="text-sm" id="footer-info">
                            <p class="pb-2 font-poppins">Subscribe our newsletter to get more notice.</p>
                            <form class="" id="subcription">
                                <input class="w-full h-12 text-sm text-gray-900 font-poppins pr-12 pl-3.5 py-0 rounded-3xl border" id="subcription-input" required="required" type="email" placeholder="Enter your email"/>
                               
                            </form>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="" id="footer-bottom">
        
        </div>
    </div>
</template>

<script>
export default {
    name: "FooterSite"
}
</script>