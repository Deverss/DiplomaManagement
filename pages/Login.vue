<template>
    <div class="flex flex-col" id="outer">
        <div class="" id="outer-inner">
            <div class="" id="login">
                <div class="relative flex grow p-x-36 p-y-16 " id="login-col-1">
                    <div class="absolute top-20 right-20 left-20 text-left text-sm font-bold" id="login-head">
                    Don't have an account?
                        <nuxt-link class="ml-1.5 text-orange-500 transition" to="/sign-up">Sign up now</nuxt-link>
                    </div>
                    <div class="m-auto w-96" id="login-wrap">
                        <div class="" id="entry">
                            <div class="mb-8 pb-8 border-b" id="entry-top">
                                <h3 class="mb-8 text text-4xl font-bold">Welcome back</h3>
                                <p class="text-gray-500" id="">Continue with Google or enter your details.</p>
                            </div>
                            <div class="" id="entry-form">
                                <div class="" id="entry-tabs">
                                    <div class="" id="nav">
                                        <button class="" id="">Email</button>
                                        <button class="" id="">Mobile</button>
                                    </div>
                                    <div class="" id="entry-container">
                                        <div class="" id="entry-item"></div>
                                    </div>
                                    <div class="" id="field-view"></div>
                                    <div class="" id="entry-foot"></div>
                                </div>
                            </div>
                            <div class="" id="entry-wrap"></div>
                        </div>
                    </div>
                </div>

                <div class="" id="login-col-2">
                
                </div>
            </div>
        </div>
    </div>
</template>
export default {
    name: 'LoginPage',
  }
  </script>