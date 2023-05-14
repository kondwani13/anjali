

<template>
  <header>
   
    <section>
        <div class="w-full relative px-6 xl:px-0">
            <img class="absolute w-full inset-0 h-full object-cover object-center" src="https://cdn.tuk.dev/assets/templates/weCare/hero2-bg.png" />
            <nav class="lg:hidden relative z-40">
                <div ref="homes" class="flex py-6 justify-between items-center px-4">
                    <div>
                        <img  @click="scrollToAnchorPoint('home')" class="w-24" src="https://i.ibb.co/m63WKs7/nlogo.png" alt="" />
                    </div>
                    <div class="flex items-center">
                        <ul id="list" class="hidden p-2 border-r bg-white absolute rounded top-0 left-0 right-0 shadow mt-16 md:mt-16">
                            <li class="flex cursor-pointer text-gray-600 text-sm leading-3 tracking-normal mt-2 py-2 hover:text-indigo-700 focus:text-indigo-700 focus:outline-none">
                                <a @click="scrollToAnchorPoint('services')">
                                    <span class="ml-2 font-bold">Services</span>
                                </a>
                            </li>
                            <li class="flex flex-col cursor-pointer text-gray-600 text-sm leading-3 tracking-normal py-2 hover:text-indigo-700 focus:text-indigo-700 focus:outline-none flex justify-center">
                                <a @click="scrollToAnchorPoint('clients')">
                                    <span class="ml-2 font-bold">Projects</span>
                                </a>
                            </li>
                            <li class="flex cursor-pointer text-gray-600 text-sm leading-3 tracking-normal py-2 hover:text-indigo-700 flex items-center focus:text-indigo-700 focus:outline-none">
                                <a @click="scrollToAnchorPoint('about')">
                                    <span class="ml-2 font-bold">About</span>
                                </a>
                            </li>
                            <li class="flex flex-col cursor-pointer text-gray-600 text-sm leading-3 tracking-normal py-2 hover:text-indigo-700 focus:text-indigo-700 focus:outline-none flex justify-center">
                                <a @click="scrollToAnchorPoint('faq')">
                                    <span class="ml-2 font-bold">Faq</span>
                                </a>
                            </li>
                        </ul>
                        <div class="xl:hidden">
                            <svg id="open" @click="MenuHandler(true)" aria-haspopup="true" aria-label="Main Menu" xmlns="http://www.w3.org/2000/svg" class="show-m-menu icon icon-tabler icon-tabler-menu" width="28" height="28" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round">
                                <path stroke="none" d="M0 0h24v24H0z"></path>
                                <line x1="4" y1="8" x2="20" y2="8"></line>
                                <line x1="4" y1="16" x2="20" y2="16"></line>
                            </svg>
                            <div id="close" class="hidden close-m-menu" @click="MenuHandler(false)">
                                <svg aria-label="Close" xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round">
                                    <path stroke="none" d="M0 0h24v24H0z" />
                                    <line x1="18" y1="6" x2="6" y2="18" />
                                    <line x1="6" y1="6" x2="18" y2="18" />
                                </svg>
                            </div>
                        </div>
                    </div>
                </div>
            </nav>
            <nav class="hidden relative z-10 w-full lg:flex justify-between items-center p-20">
                <div ref="home" class="w-1/6">
                    <a>
                        <img class="" src="https://i.ibb.co/m63WKs7/nlogo.png" />
                    </a>
                </div>
                <div class="w-5/6">
                    <div class="flex items-center justify-end">
                        <ul class="text-gray-800 flex items-center leading-none">
                            <li>
                                <button @click="scrollToAnchorPoint('services')">Services</button>
                            </li>
                            <li class="ml-4">
                                <button @click="scrollToAnchorPoint('clients')">Projects</button>
                            </li>
                            <li class="ml-4">
                                <button @click="scrollToAnchorPoint('about')">About</button>
                            </li>
                            <li class="ml-3">
                                <button @click="scrollToAnchorPoint('faq')">Faq</button>
                            </li>
                        </ul>
                        <div class="pl-40">
                           <img class="w-20 h-20 " src="https://i.ibb.co/h90d3hV/app.png" alt="app" />
                        </div>
                    </div>
                </div>
            </nav>
            <div class="pt-32 lg:flex items-center relative z-10 container mx-auto">
                <div class="w-full lg:w-1/2 h-full lg:pr-10 xl:pr-0">
                    <img class="mx-auto" src="https://i.ibb.co/j630m23/hero2.png" />
                </div>
                <div class="w-full lg:w-1/2 h-full z-10">
                    <p class="text-indigo-500 uppercase font-bold text-center pt-6 text-2xl mb-4">Passion never fails</p>
                    <h1 class="text-gray-900 text-3xl text-center md:text-7xl mb-8">In service to the people.</h1>
                    <p class="text-gray-800 text-center font-regular mb-8">Hi I'm Anjali Gupta an independent and self motivated experienced business development manager with vast valuable industry knowledge and passion for management. I'm a result oriented person with a proven track record for improving the market position of companies and maximizing opportunities for their financial growth.</p>
                    <div class="bg-white py-4 px-4 flex flex-col sm:flex-row justify-start sm:justify-between items-start sm:items-center shadow-lg rounded-lg">
                        <div class="sm:flex items-center py-2">
                            <div class="flex items-center">
                                <svg xmlns="http://www.w3.org/2000/svg" class="text-indigo-500 icon icon-tabler icon-tabler-user" width="16" height="16" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round">
                                    <path stroke="none" d="M0 0h24v24H0z" fill="none" />
                                    <circle cx="12" cy="7" r="4" />
                                    <path d="M6 21v-2a4 4 0 0 1 4 -4h4a4 4 0 0 1 4 4v2" />
                                </svg>
                                <p class="leading-none tracking-normal text-gray-800 ml-2.5">Community development</p>
                            </div>
                            <div class="flex items-center sm:mx-4 xl:mx-14 my-6 lg:my-0">
                                <svg xmlns="http://www.w3.org/2000/svg" class="text-indigo-500 icon icon-tabler icon-tabler-layout-bottombar" width="16" height="16" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round">
                                    <path stroke="none" d="M0 0h24v24H0z" fill="none" />
                                    <rect x="4" y="4" width="16" height="16" rx="2" />
                                    <line x1="4" y1="15" x2="20" y2="15" />
                                </svg>
                                <p class="leading-none tracking-normal text-gray-800 ml-2.5">Entreprenuership</p>
                            </div>
                            <div class="flex items-center">
                                <svg xmlns="http://www.w3.org/2000/svg" class="text-indigo-500 icon icon-tabler icon-tabler-flag" width="16" height="16" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round">
                                    <path stroke="none" d="M0 0h24v24H0z" fill="none" />
                                    <line x1="5" y1="5" x2="5" y2="21" />
                                    <line x1="19" y1="5" x2="19" y2="14" />
                                    <path d="M5 5a5 5 0 0 1 7 0a5 5 0 0 0 7 0" />
                                    <path d="M5 14a5 5 0 0 1 7 0a5 5 0 0 0 7 0" />
                                </svg>
                                <p class="leading-none tracking-normal text-gray-800 ml-2.5">Lusaka</p>
                            </div>
                        </div>
                       
                    </div>
                </div>
            </div>
        </div>
    </section>
     </header>
     <div class="pt-4">
     <stats />
     </div>

     <div ref="services" class="py-20 2xl:px-0 lg:px-12 px-4 2xl:mx-auto 2xl:container bg-white" style="height: 1000px">
        <div class="md:flex items-center justify-between w-full bg-white">
        
        
            <div class="xl:w-1/3 md:w-1/2 w-full lg:px-20 px-4">
                <h1 role="heading" class="focus:outline-none md:w-60 font-bold md:text-6xl text-4xl leading-tight text-gray-800">Services<span class="font-normal italic"> offered </span></h1>
                <p role="contentinfo" class="focus:outline-none text-base leading-6 mt-8 text-gray-600 2xl:pr-24 xl:pr-0 pr-12">My life's work has been centered around community development and progress, that being so I strongly believe that we can achieve more when we mobilize ourselves in teams around a common goal.</p>
                <p role="contentinfo" class="focus:outline-none pt-2 text-base leading-6  text-gray-600 2xl:pr-24 xl:pr-0 pr-12">I offer a soft skills development platform which is open to anybody that would like to take part, I aim at equipping Zambian women with cross culture methods of doing things. For example I teach young women how to prepare Indian food etc...</p>

                <div class="mt-6 overflow-x-hidden">
                    <div class="lg:pl-36 lg:pr-16 pl-4 bg-blue-back1 w-full inline-flex pb-8 pt-6 lg:space-x-24 "> 

      <button  @click="activeTab = 'Passion'" class=" lg:text-4xl text-indigo-800 hover:text-white px-2">management systems</button>
       <button  @click="activeTab = 'Picture'" class=" lg:text-4xl text-indigo-800 hover:text-white px-2">ERP'S</button>
       <button  @click="activeTab = 'Website'" class=" lg:text-4xl text-indigo-800 hover:text-white px-2">Digital Marketing</button>
       <button  @click="activeTab = 'Apps'" class=" lg:text-4xl text-indigo-800 hover:text-white px-2">IT consultance</button>
        
    </div>
                </div>
            </div>
            <div class="mb-8 pb-6 xl:w-4/6 md:w-1/2 w-full xl:pl-48 lg:px-20 px-4">
               <component :is="activeTab" />
            </div>
        </div>
    </div>

   

    

   <div class="pt-28 mt-36" ref="clients">
    <project /> 
   </div>
   <div ref="about">
    <about />
    </div>
    <div ref="faq">
    <faq />
    </div>
    <!-- footer -->
    <div class="bg-gray-800">
        <div class="px-4 py-9 md:px-6 md:py-12 lg:px-20 lg:py-12">
            <div class="flex flex-col md:flex-row md:justify-between pb-10">
                <div class="flex flex-col items-center">
                    <button class="w-full md:w-auto px-24 py-2 bg-white border rounded-md text-xl font-semibold leading-tight text-gray-800 hover:bg-gray-200 focus:ring-2 focus:outline-none focus:ring-gray-200 focus:ring-opacity-50">Get started</button>
                    <p class="pt-2 text-sm leading-none text-gray-300 cursor-pointer hover:underline"></p>
                </div>
                <div>
                    <p class="w-72 pt-9 md:py-0 text-sm leading-tight text-gray-300">09:00 AM to 6 PM, ibex hill 123/32, Lusaka</p>
                </div>
            </div>
 
            <div class="w-full px-8 border-white border rounded-md flex flex-col justify-start md:flex-row md:justify-between lg:justify-center gap-2 md:gap-20 py-6">
                <p class="text-sm leading-none text-gray-300"></p>
                <div class="flex justify-start gap-4">
                   <img src="https://tuk-cdn.s3.amazonaws.com/can-uploader/footer_4-svg1.svg" alt="Email">
                    <p class="text-sm leading-none text-gray-300">anjaligupta@gmail.com</p>
                </div>
            </div>

            <div class="pt-10 flex flex-col xl:flex-row justify-between">
                <div class="flex flex-col md:gap-10">
                    <div class="flex items-start w-full">
                        <div class="pb-10 md:pb-0">
                        <h3 class="text-xl cursor-default font-semibold leading-tight text-white mb-8">Product</h3>
                            <p class="text-sm cursor-pointer leading-none text-gray-300 mb-6">Garlic paste</p>
                            <p class="text-sm cursor-pointer leading-none text-gray-300 mb-6">Ginger powder</p>
                            <p class="text-sm cursor-pointer leading-none text-gray-300 mb-6">onion powder...</p>
                        </div>
                        <div class="pb-10 md:pb-0 2xl:pl-20 pl-16">
                            <h3 class="text-xl cursor-default font-semibold leading-tight text-white mb-8">Support</h3>
                            <p class="text-sm cursor-pointer leading-none text-gray-300 mb-6">Generate lead</p>
                            <p class="text-sm cursor-pointer leading-none text-gray-300 mb-6">Size Guide</p>
                            <p class="text-sm cursor-pointer leading-none text-gray-300 mb-6"></p>
                            <p class="text-sm cursor-pointer leading-none text-gray-300 mb-6"></p>
                        </div>
                        <div class="pb-10 md:pb-0 2xl:pl-20 pl-16 md:block hidden">
                            <h3 class="text-xl cursor-default font-semibold leading-tight text-white mb-8">Solutions</h3>
                            <p class="text-sm cursor-pointer leading-none text-gray-300 mb-6">Generate Lead</p>
                            <p class="text-sm cursor-pointer leading-none text-gray-300 mb-6">Self knowledge</p>
                            <p class="text-sm cursor-pointer leading-none text-gray-300 mb-6">Work from home</p>
                            <p class="text-sm cursor-pointer leading-none text-gray-300 mb-6">Engage customers</p>
                            <p class="text-sm cursor-pointer leading-none text-gray-300 mb-6">Boost online sales</p>
                        </div>
                        
                    </div>
                    <div class="flex items-start">
                        <div class="pb-10 md:pb-0 md:hidden">
                            <h3 class="text-xl cursor-default font-semibold leading-tight text-white mb-8">Solutions</h3>
                            <p class="text-sm cursor-pointer leading-none text-gray-300 mb-6">Generate Lead</p>
                            <p class="text-sm cursor-pointer leading-none text-gray-300 mb-6">Self knowledge</p>
                            
                            <p class="text-sm cursor-pointer leading-none text-gray-300 mb-6">Engage customers</p>
                            <p class="text-sm cursor-pointer leading-none text-gray-300 mb-6">Boost online sales</p>
                        </div>
                        <div class="pb-10 md:pb-0 2xl:pl-20 pl-16">
                            <h3 class="text-xl cursor-default font-semibold leading-tight text-white pb-8">Entreprenuer</h3>
                            <p class="text-sm cursor-pointer leading-none text-gray-300 pb-6">Online Marketer</p>
                            <p class="text-sm cursor-pointer leading-none text-gray-300 pb-6">Marketing management</p>
                            <p class="text-sm cursor-pointer leading-none text-gray-300 pb-6">Email marketing</p>
                        </div>
                    </div>
                    <div class="flex items-start w-full">
                       
                       
                        <div class="2xl:pl-20 md:pl-16 md:block hidden">
                            <h3 class="text-xl cursor-default font-semibold leading-tight text-white pb-8">Get responce</h3>
                            <p class="text-sm cursor-pointer leading-none text-gray-300 pb-6">Career</p>
                            <p class="text-sm cursor-pointer leading-none text-gray-300 pb-6">Api docs</p>
                            <p class="text-sm cursor-pointer leading-none text-gray-300 pb-6">Accessibility</p>
                        </div>
                    </div>
                   
                </div>

                <div class="pt-16 md:pt-12 lg:pt-0">
                    <h3 class="text-xl font-semibold leading-tight text-white">Blog</h3>
                    <div class="pt-8 mb-6 flex justify-center cursor-pointer items-center flex-col md:flex-row md:justify-start gap-6">
                        <img class="hidden lg:block" src="https://i.ibb.co/NsH4JJX/blog1.png" alt="a workspace" />
                        <img class="block lg:hidden" src="https://i.ibb.co/NsH4JJX/blog1.png" alt="a workspace" />
                        <p class="text-center md:text-left text-base font-semibold cursor-pointer leading-normal text-gray-100">Why you should self educate</p>
                    </div>
                    <div class="mb-6 flex justify-center cursor-pointer items-center flex-col md:flex-row md:justify-start gap-6">
                        <img class="hidden lg:block" src="https://i.ibb.co/L8ZXnrC/fhands.png" alt="a woman" />
                        <img class="block lg:hidden" src="https://i.ibb.co/L8ZXnrC/fhands.png" alt="a woman" />
                        <p class="text-center md:text-left text-base font-semibold cursor-pointer leading-normal text-gray-100">Importance of women empowerment</p>
                    </div>
                    <div class="mb-6 flex justify-center cursor-pointer items-center flex-col md:flex-row md:justify-start gap-6">
                        <img class="hidden lg:block" src="https://i.ibb.co/WKq13ry/ginderp.png" alt="a workspace" />
                        <img class="block lg:hidden" src="https://i.ibb.co/WKq13ry/ginderp.png" alt="a workspace" />
                        <p class="text-center md:text-left text-base font-semibold leading-normal text-gray-100">the health benefits of ginger powder</p>
                    </div>
                    <div class="flex items-center md:justify-start justify-center">
                        <button class="pt-8 hover:underline text-base font-medium leading-none text-white cursor-pointer">View all posts</button>
                    </div>
                </div>
            </div>

            <div class="pt-10 lg:pt-24 flex justify-center md:justify-start gap-12">
               <img src="https://tuk-cdn.s3.amazonaws.com/can-uploader/footer_4-svg2.svg" alt="facebook">
                <img src="https://tuk-cdn.s3.amazonaws.com/can-uploader/footer_4-svg3.svg" alt="twitter">
                <img src="https://tuk-cdn.s3.amazonaws.com/can-uploader/footer_4-svg4.svg" alt="instagram">
                <img src="https://tuk-cdn.s3.amazonaws.com/can-uploader/footer_4-svg5.svg" alt="youtube">
               <img src="https://tuk-cdn.s3.amazonaws.com/can-uploader/footer_4-svg6.svg" alt="pintrest">
            </div>
        </div>
    </div>

    <!-- footer end -->
      

     
    
  <button  @click="scrollToAnchorPoint('homes')"
        class="fixed z-50 bottom-10 right-8 w-20 h-20 rounded-full flex justify-center items-center text-white text-4xl hover:bg-blue-700 hover:drop-shadow-2xl hover:animate-bounce duration-300">
        <img class="z-50" src="https://i.ibb.co/MPdQjJV/up.png" alt="up" /></button>


  <RouterView />
</template>

<script>
import Airtable from 'airtable';
Airtable.configure({
    endpointUrl: 'https://api.airtable.com',
    apiKey: import.meta.env.VITE_AIRTABLE_API_KEY
});
var base = Airtable.base(import.meta.env.VITE_BASE);

base('Table 1').select({
    // Selecting the first 3 records in Grid view:
    maxRecords: 3,
    view: "Grid view"
}).eachPage(function page(records, fetchNextPage) {
    // This function (`page`) will get called for each page of records.

    records.forEach(function(record) {
        console.log('Retrieved', record.get('name'));
    });

    // To fetch the next page of records, call `fetchNextPage`.
    // If there are more records, `page` will get called again.
    // If there are no more records, `done` will get called.
    fetchNextPage();

}, function done(err) {
    if (err) { console.error(err); return; }
});
import { RouterLink, RouterView } from 'vue-router'
import AnimCount from './components/AnimCount.vue'
import Project from './components/Project.vue'
import Footer from './components/Footer.vue'
import Faq from './components/Faq.vue'
import Stats from './components/Stats.vue'
import About from './components/About.vue'
import Passion from './components/Passion.vue'
import Picture from './components/Picture.vue'
import Website from './components/Website.vue'
import Apps from './components/Apps.vue'


 

export default {
    name: "Index",
    components: {AnimCount, Project, Footer, Faq, Stats, About, Passion, Picture, Website, Apps},

  
    data() {
      return {
       
        activeTab: Passion,
        
       
        
      }
    },
    methods: {

        scrollToAnchorPoint(refName) {
            const el = this.$refs[refName]
            el.scrollIntoView({ behavior: 'smooth'})
        },
        MenuHandler(flag) {
            if (flag) {
                document.getElementById("list").classList.add("top-100");
                document.getElementById("list").classList.remove("hidden");
                document.getElementById("close").classList.remove("hidden");
                document.getElementById("open").classList.add("hidden");
            } else {
                document.getElementById("list").classList.remove("top-100");
                document.getElementById("list").classList.add("hidden");
                document.getElementById("close").classList.add("hidden");
                document.getElementById("open").classList.remove("hidden");
            }
        },
    },
};



    

</script>



<style scoped>
/* Top menu */
.top-100 {
    animation: slideDown 0.5s ease-in-out;
}
@keyframes slideDown {
    0% {
        top: -50%;
    }
    100% {
        top: 0;
    }
}
* {
    outline: none !important;
    -webkit-tap-highlight-color: rgba(0, 0, 0, 0);
    -webkit-tap-highlight-color: transparent;
}



</style>


