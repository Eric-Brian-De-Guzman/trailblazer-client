<script setup>
import { RouterView } from 'vue-router'
import { library } from '@fortawesome/fontawesome-svg-core'
import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome'
import { faRightFromBracket, faUser } from '@fortawesome/free-solid-svg-icons'
import { faCircleExclamation } from '@fortawesome/free-solid-svg-icons'
import { faGear } from '@fortawesome/free-solid-svg-icons'


import { onMounted } from 'vue'
import { initFlowbite } from 'flowbite'

// initialize components based on data attribute selectors
onMounted(() => {
    initFlowbite();
})
library.add(faGear)
library.add(faUser)
library.add(faCircleExclamation)
</script>

<template>



<nav class="bg-white border-gray-200 shadow-md dark:bg-gray-900">
  <div class="max-w-screen-xl flex flex-wrap items-center justify-between mx-auto p-4">
  <a href="https://flowbite.com/" class="flex items-center">

      <span class="self-center text-2xl font-semibold whitespace-nowrap dark:text-white">Trailblazer Community Dashboard</span>
  </a>
  <div class="flex items-center md:order-2">
      <button type="button" class="w-full flex" id="user-menu-button" aria-expanded="false" data-dropdown-toggle="user-dropdown" data-dropdown-placement="bottom">
       <div class="bg-black  w-6 h-6 rounded-full">
        <font-awesome-icon  :icon="faUser"  class="fa-solid fa-user  " style="color: #ffffff;"/></div>
         <span class="ml-2  whitespace-nowrap dark:text-white">Administrator</span>
      </button>
     
      <!-- Dropdown menu -->
      <div class="z-50  px-5 hidden my-4 text-base list-none bg-white divide-y divide-gray-100 rounded-lg shadow dark:bg-gray-700 dark:divide-gray-600" id="user-dropdown">
        
        <ul class="py-2" aria-labelledby="user-menu-button">
          <li>
            <a href="#" class="block px-4 py-2 text-md text-gray-700 hover:rounded-xl hover:text-white hover:bg-gray-900 dark:hover:bg-gray-600 dark:text-gray-200 dark:hover:text-white"><font-awesome-icon  :icon="faUser"  class="fa-solid fa-user mr-2 " />Administrator</a>
          </li>
          <li>
            <a href="#" class="block px-4 py-2 text-md text-gray-700 hover:rounded-xl hover:text-white hover:bg-gray-900 dark:hover:bg-gray-600 dark:text-gray-200 dark:hover:text-white"><font-awesome-icon  :icon="faGear"  class="fa-solid fa-gear  mr-2" />Settings</a>
          </li>
         
          <li>
            <a href="#" class="block px-4 py-2 text-md text-gray-700 hover:rounded-xl hover:text-white hover:bg-gray-900 dark:hover:bg-gray-600 dark:text-gray-200 dark:hover:text-white"><font-awesome-icon  :icon="faRightFromBracket"  class="fa-solid fa-user mr-2 " />Sign out</a>
          </li>
        </ul>
      </div>
      <button data-collapse-toggle="navbar-user" type="button" class="inline-flex items-center p-2 w-10 h-10 justify-center text-sm text-gray-500 rounded-lg md:hidden hover:bg-gray-100 focus:outline-none focus:ring-2 focus:ring-gray-200 dark:text-gray-400 dark:hover:bg-gray-700 dark:focus:ring-gray-600" aria-controls="navbar-user" aria-expanded="false">
        <span class="sr-only">Open main menu</span>
        <svg class="w-5 h-5" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 17 14">
            <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M1 1h15M1 7h15M1 13h15"/>
        </svg>
    </button>
  </div>
  
  </div>
</nav>



  <RouterView />
  


</template>

<style>
body{background: #F9F9F9;}
</style>