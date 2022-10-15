<template>
    <div class="w-full bg-gray-200 dark:bg-gray-900 mt-10 py-10">
        <div class="container mx-auto px-6 flex items-start justify-center">
            <div class="w-full">
                <!-- Card is full width. Use in 12 col grid for best view. -->
                <!-- Card code block start -->
                <div class="mx-auto w-full p-5 lg:p-10 bg-white dark:bg-gray-800 shadow rounded">
                    <div class="flex flex-col lg:flex-row items-start lg:items-center mb-8">
                        <h1 class="mr-12 text-xl lg:text-2xl text-gray-800 dark:text-gray-100 font-bold lg:w-1/2">Main corporate projets</h1>
                        
                    </div>
                    <div class="flex flex-col lg:flex-row items-start lg:items-center">
                        <div class="w-full lg:w-1/2 pr-0 lg:pr-48">
                            <div class="flex items-center">
                                <div class="w-12 h-12 rounded">
                                    <img class="w-full h-full overflow-hidden object-cover rounded object-center" src="https://i.postimg.cc/qM50xPxS/grand.png" alt="logo" />
                                </div>
                                <div class="ml-2">
                                    <h5 class="text-gray-800 dark:text-gray-100 font-medium text-base">Grand tech</h5>
                                    <p class="text-gray-600 dark:text-gray-400 text-xs font-normal">Lusaka, Zambia</p>
                                </div>
                            </div>
                            
                            <p class="mt-5 text-sm text-gray-600 dark:text-gray-400 font-normal">Grand tech is a consultancy company that helps new startups and existing companies organize there company in the legal, tech, and finace aspects.</p>
                        </div>
                        <div class="flex flex-col md:flex-row items-start md:items-center">
                            <div class="mt-4 lg:mt-0 mr-0 xl:mr-8 text-sm bg-indigo-100 text-indigo-700 dark:text-indigo-600 rounded font-medium py-2 w-48 flex justify-center">Start Date: 22 Jun, 2020</div>
                            <div class="mt-4 lg:mt-0 mr-0 lg:mr-4 xl:mr-8 text-sm bg-green-100 text-green-500 rounded font-medium py-2 w-48 flex justify-center">On going project</div>
                        </div>
                        <h1 class="hidden-lg pt-4 mr-12 text-xl lg:text-2xl text-gray-800 dark:text-gray-100 font-bold lg:w-1/2">We provide consultancy in;</h1>
                        <div class="lg:pl-8 w-full lg:w-1/2 flex flex-col lg:flex-row items-start lg:items-center">
                            <div class="mr-12 flex lg:block items-center lg:mr-6 xl:mr-12 mt-5 lg:mt-0">
                                <h2 class="text-gray-600 dark:text-gray-400 font-bold text-xl lg:text-2xl leading-6 mb-1 lg:text-center">1.</h2>
                                <p class="ml-2 lg:ml-0 text-gray-800 dark:text-gray-100 text-base leading-5 text-center">Software and digital Marketing</p>
                            </div>
                            <div class="mr-12 flex lg:block lg:mr-6 xl:mr-12 mt-5 lg:mt-0">
                                <h2 class="text-gray-600 dark:text-gray-400 font-bold text-xl lg:text-2xl leading-6 mb-1 lg:text-center">2.</h2>
                                <p class="ml-2 lg:ml-0 text-gray-800 dark:text-gray-100 text-base leading-5 text-center">Accountancy</p>
                            </div>
                            <div class="mt-5 flex lg:block lg:mt-0">
                                <h2 class="text-gray-600 dark:text-gray-400 font-bold text-xl lg:text-2xl leading-6 mb-1 lg:text-center">3.</h2>
                                <p class="ml-2 lg:ml-0 text-gray-800 dark:text-gray-100 text-base leading-5 text-center">Law</p>
                            </div>
                        </div>
                    </div>
                    <div class="relative">
                        <hr class="mt-8 mb-8 lg:mb-10 h-1 rounded bg-gray-200" />
                        <hr class="absolute top-0 h-1 w-2/3 rounded bg-indigo-400" />
                    </div>
                    <div class="flex flex-col lg:flex-row items-start lg:items-center">
                        <div class="flex flex-col lg:flex-row w-full lg:w-2/3 items-start lg:items-center mb-8 lg:mb-0">
                        <h1 class="hidden-lg pt-4 pb-4 mr-12 text-xl lg:text-2xl text-gray-800 dark:text-gray-100 font-bold lg:w-1/2">Clients</h1>
                            <div class="mr-24 flex lg:block flex-row-reverse items-center mb-4 lg:mb-0">
                                <h3 class="text-indigo-700 dark:text-indigo-600 leading-6 text-base">tech company</h3>
                                <h2 class="mr-2 lg:mr-0 text-gray-600 dark:text-gray-400 text-base lg:text-2xl font-bold">Protolog</h2>
                            </div>
                            <div class="mr-24 flex lg:block flex-row-reverse items-center mb-4 lg:mb-0">
                                <h3 class="text-indigo-700 dark:text-indigo-600 leading-6 text-base">Agro-processing</h3>
                                <h2 class="mr-2 lg:mr-0 text-gray-600 dark:text-gray-400 text-base lg:text-2xl font-bold">Nzuri</h2>
                            </div>
                            <div class="flex lg:block flex-row-reverse items-center">
                                <h3 class="text-indigo-700 dark:text-indigo-600 leading-6 text-base">Logistics company</h3>
                                <h2 class="mr-2 lg:mr-0 text-gray-600 dark:text-gray-400 text-base lg:text-2xl font-bold">Bee & Dee</h2>
                            </div>
                        </div>
                        <div class="flex items-center w-full lg:w-1/3 justify-start lg:justify-end">
                            <div class="border-2 border-white dark:border-gray-700 shadow rounded-full w-10 h-10">
                                <img class="w-full h-full overflow-hidden object-cover rounded-full" src="https://dh-ui.s3.amazonaws.com/assets/webapp/layout/grid_cards/grid_card8.jpg" alt="avatar" />
                            </div>
                            <div class="-ml-4 border-2 border-white dark:border-gray-700 shadow rounded-full w-10 h-10">
                                <img class="w-full h-full overflow-hidden object-cover rounded-full" src="https://dh-ui.s3.amazonaws.com/assets/webapp/layout/grid_cards/grid_card9.jpg" alt="avatar" />
                            </div>
                            <div class="-ml-4 border-2 border-white dark:border-gray-700 shadow rounded-full w-10 h-10">
                                <img class="w-full h-full overflow-hidden object-cover rounded-full" src="https://dh-ui.s3.amazonaws.com/assets/webapp/layout/grid_cards/grid_card10.jpg" alt="avatar" />
                            </div>
                            <div class="-ml-4 border-2 border-white dark:border-gray-700 shadow rounded-full w-10 h-10">
                                <img class="w-full h-full overflow-hidden object-cover rounded-full" src="https://dh-ui.s3.amazonaws.com/assets/webapp/layout/grid_cards/grid_card11.jpg" alt="avatar" />
                            </div>
                            <div class="-ml-4 border-2 border-white dark:border-gray-700 shadow rounded-full w-10 h-10">
                                <img class="w-full h-full overflow-hidden object-cover rounded-full" src="https://dh-ui.s3.amazonaws.com/assets/webapp/layout/grid_cards/grid_card12.jpg" alt="avatar" />
                            </div>
                        </div>
                    </div>
                </div>
                <!-- Card code block end -->
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "Project",
};
</script>
