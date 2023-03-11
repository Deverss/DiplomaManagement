<template>
    <div>
        <navbar />
        <div>
            <div class="max-w-screen-xl w-full mx-auto " id="section">
                <div class="py-32 flex items-start max-w-screen-xl" id="container">
                    <div class="flex-grow-0 flex-shrink-0 pr-32 " id="upload-wrapper">
                        <div class="mb-10" id="upload-head">
                            <div class="mr-auto font-poppins text-5xl font-bold" id="upload-title">Upload <br>new certificate</div>
                            <!-- <NuxtLink class="" id="upload-switch" to="#">Switch to bulk upload</NuxtLink> -->
                        </div>
                        <form class="" id="upload-form" action>
                            <div class="mb-10 pb-10" id="upload-detail-list">
                                <div class="mb-10" id="upload-detail-item">
                                    <div class="text-base leading-normal font-bold font-poppins" id="upload-detail-category">
                                        Upload file
                                    </div>
                                    <div class="mt-1 text-xs text-gray-600 font-poppins" id="upload-detail-note">Drag or choose your file to upload</div>
                                    <div class="relative flex flex-col justify-center items-center h-48 mt-4 overflow-hidden bg-gray-100 rounded-2xl" id="upload-detail-file">
                                        <label for="upload-detail-load">
                                            <input class="absolute top-0 left-0 opacity-0" id="upload-detail-load" type="file" accept=".pdf" @change="onFileSelected"/>
                                            <div class="mb-2" id="upload-detail-icon">
                                            <svg class width="24" height="24" viewBox="0 0 16 16" fill="inherit">
                                                <path d="M10.229.667c.707 0 1.386.281 1.886.781l1.105 1.105c.5.5.781 1.178.781 1.886v8.229c0 1.473-1.194 2.667-2.667 2.667H4.667C3.194 15.334 2 14.14 2 12.667V3.334C2 1.861 3.194.667 4.667.667h5.562zM9.333 2H4.667c-.693 0-1.263.529-1.327 1.205l-.006.128v9.333c0 .693.529 1.263 1.205 1.327l.128.006h6.667c.693 0 1.263-.529 1.327-1.205l.006-.128V5.334h-1.333a2 2 0 0 1-1.995-1.851l-.005-.149V2zM7.745 6.051c.242-.1.53-.052.727.145h0l2 2c.26.26.26.682 0 .943s-.682.26-.943 0h0l-.862-.862v3.057c0 .368-.298.667-.667.667s-.667-.298-.667-.667h0V8.276l-.862.862c-.26.26-.682.26-.943 0s-.26-.682 0-.943h0l2-2c.064-.064.138-.112.216-.145zm2.922-3.977v1.259c0 .368.298.667.667.667h1.259c-.065-.188-.173-.361-.317-.505l-1.105-1.105c-.144-.144-.317-.251-.505-.317z"></path>
                                            </svg>
                                            </div>
                                            <div class="text-xs text-gray-600" id="upload-detail-format">Only accept PDF file</div>
                                        </label>
                                    </div>
                                </div>

                                <div class="" id="upload-detail-item">
                                    <div class="text-base leading-normal font-bold font-poppins" id="upload-detail-category">
                                        Certificate detail
                                    </div>
                                    <div class="mt-8" id="upload-detail-fieldset">
                                    <!-- FIELD -->
                                        <div class="mb-8" id="upload-detail-field">
                                            <div class="mb-3 text-xs leading-none font-bold uppercase text-gray-500" id="text-input">Student's full name</div>
                                            <div class="">
                                                <input class="w-full h-12 text-sm font-medium text-gray-900 px-3.5 py-0 rounded-xl border-2 font-poppins" name="full-name" id="full-name" type="text" placeholder="Input student's name" required/>
                                            </div>
                                        </div>
                                    <!-- FIELD -->
                                    <!-- FIELD -->
                                    <div class="mb-8" id="upload-detail-field">
                                            <div class="mb-3 text-xs leading-none font-bold uppercase text-gray-500" id="text-input">Email</div>
                                            <div class="">
                                                <input class="w-full h-12 text-sm font-medium text-gray-900 px-3.5 py-0 rounded-xl border-2 font-poppins" name="email" type="email" id="email" placeholder="Input student's name" required/>
                                            </div>
                                        </div>
                                    <!-- FIELD -->
                                    <!-- FIELD -->
                                    <div class="mb-8 flex" id="upload-detail-row">
                                        <div class="flex-grow-0 flex-shrink-0 w-calc(33.333% - 20px) flex flex-col items-center" id="upload-detail-col">
                                            <div class="" id="upload-detail-field">
                                                <div class="mb-3 text-xs leading-none font-bold uppercase text-gray-500" id="text-input-label">Grade</div>
                                                <div>
                                                    <input class="w-full h-12 text-sm font-medium text-gray-900 py-0 px-3.5 rounded-xl border-2 font-poppins" id="text-input-input" name="grade" type="text" placeholder="20" required/>
                                                </div>
                                            </div>
                                        </div>
                                        <div class="flex-grow-0 flex-shrink-0 w-calc(33.333% - 20px) flex flex-col items-center ml-4" id="upload-detail-col">
                                            <div class="" id="upload-detail-field">
                                                <div class="mb-3 text-xs leading-none font-bold uppercase text-gray-500" id="text-input-label">In Class</div>
                                                <div>
                                                    <input class="w-full h-12 text-sm font-medium text-gray-900 py-0 px-3.5 rounded-xl border-2 font-poppins" id="text-input-input" name="class" type="text" placeholder="20" required/>
                                                </div>
                                            </div>
                                        </div>
                                        <div class="flex-grow-0 flex-shrink-0 w-calc(33.333% - 20px) flex flex-col items-center ml-4" id="upload-detail-col">
                                            <div class="" id="upload-detail-field">
                                                <div class="mb-3 text-xs leading-none font-bold uppercase text-gray-500" id="text-input-label">Finish year</div>
                                                <div>
                                                    <input class="w-full h-12 text-sm font-medium text-gray-900 py-0 px-3.5 rounded-xl border-2 font-poppins" id="text-input-input" name="finish-year" type="number" placeholder="2017" max="2025" required/>
                                                </div>
                                            </div>
                                        </div>
                                    </div>
                                    <!-- FIELD -->
                                    
                                    
                                </div>
                            </div>
                        </div>
                        <div class="flex items-center" id="Upload-details-foot">
                            <button class="inline-flex justify-center items-center h-12 px-6 bg-blue-500 rounded-full font-medium text-lg text-white transition duration-200" id="upload-details-button" type="submit">
                                <span>Create</span>
                                <svg class="w-4 h-4 ml-2 inline-flex items-center" viewBox="0 0 16 16" fill="white" stroke="currentColor">
                                    <path d="M10.39 3.765c.464-.375 1.187-.349 1.615.057l3.692 3.5a.91.91 0 0 1 0 1.357l-3.692 3.5c-.428.406-1.151.431-1.615.057s-.493-1.007-.065-1.413L12.247 9H1.143C.512 9 0 8.552 0 8s.512-1 1.143-1h11.104l-1.922-1.822c-.428-.406-.399-1.038.065-1.413z"/>
                                </svg>
                            </button>
                        </div>
                    </form>
                </div>
                <div class="flex-shrink-0 w-96 ml-auto" id="upload-preview">
                    <div class="p-12 bg-fcfcfd shadow-lg rounded-2xl" id="preview-inner">
                        <div class="mb-6 text-3xl font-semibold leading-8 tracking-tighter" id="preview-info">Preview</div>
                        <div>
                            <div class="relative rounded-xl overflow-hidden" id="preview-preview">
                                <img class="w-full align-middle" src="https://images.unsplash.com/photo-1584445584400-1a7cc5de77ae?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=760&q=80" alt="card"/>
                            </div>
                            <div class="py-4 text-gray-700" id="preview-link">
                                <div class="flex items-start mb-12" id="preview-line">
                                    <div class=" text-base font-bold leading-6 text-gray-900" id="preview-fullname">Mai The Son</div>
                                    <div class="flex-shrink-0 ml-auto rounded border border-green-500 px-2 text-xs leading-6 font-bold uppercase text-green-500" id="preview-class">20GIT</div>
                                </div>
                            </div>
                        </div>
                        <button class="inline-flex items-center mt-6 text-base font-bold leading-1 text-gray-500 transition-colors duration-200 ease-in-out" id="preview-clear">
                            <svg class width="24" height="24" viewBox="0 0 16 16" fill="inherit">
                                <path d="M8 1.333A6.67 6.67 0 0 1 14.666 8 6.67 6.67 0 0 1 8 14.666 6.67 6.67 0 0 1 1.333 8 6.67 6.67 0 0 1 8 1.333zm0 1.333C5.054 2.666 2.666 5.054 2.666 8S5.054 13.333 8 13.333 13.333 10.945 13.333 8 10.945 2.666 8 2.666zm2.471 2.862c.26.26.26.682 0 .943L8.942 8l1.529 1.529c.26.26.26.682 0 .943s-.682.26-.943 0L8 8.942l-1.529 1.529c-.26.26-.682.26-.943 0s-.26-.682 0-.943L7.057 8 5.528 6.471c-.26-.26-.26-.682 0-.943s.682-.26.943 0L8 7.057l1.529-1.529c.26-.26.682-.26.943 0z" />
                            </svg>
                            Clear all
                        </button>
                    </div>
                </div>
                </div>
            </div>
            <Footer />
        </div>
    </div>
</template>
<script>
    
</script>