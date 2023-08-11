<script setup>
import UserTable from '../components/HomeView/UserTable.vue';
import { library } from '@fortawesome/fontawesome-svg-core'
import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome'
import { faRightFromBracket, faUserTag, faUserClock, faUserCheck, faUserGroup, faCamera } from '@fortawesome/free-solid-svg-icons'
import { faCircleExclamation } from '@fortawesome/free-solid-svg-icons'
import { faGear } from '@fortawesome/free-solid-svg-icons'
library.add(faCamera)
library.add(faUserGroup)
library.add(faUserCheck)
library.add(faUserClock)
library.add(faUserTag)
library.add(faCircleExclamation)
</script>

<template>
  <div class="w-3/4 mx-auto">

    <div class="grid grid-cols-6 gap-3">
<div class="col-span-6 mt-5"><span class="text-4xl font-medium">Statistics</span></div>
<div></div>
<div class="flex h-36 w-full rounded-lg bg-white p-4 shadow-md">
  <div>
    <h2 class="mb-2 text-xl font-semibold">Pending Invites</h2>
    <div class="flex">
       <font-awesome-icon  :icon="faUserClock"  class="fa-solid fa-user mt-5 h-12" style="color: #ec5500;"/>
      <p class="mt-4 text-right">
        <span class="ml-6 font-bold text-5xl text-blue-500">126</span>
      </p>
    </div>
  </div>
</div>

<div class="flex h-36 w-full rounded-lg bg-white p-4 shadow-md">
  <div>
    <h2 class="mb-2 text-xl font-semibold">Paid, not Arrive</h2>
    <div class="flex">
      <font-awesome-icon  :icon="faUserTag"  class="fa-solid fa-user mt-5 h-12" style="color: #1e6ecc;"/>
      <p class="mt-4 text-right">
        <span class="ml-6 font-bold text-5xl text-blue-500">126</span>
      </p>
    </div>
  </div>
</div>

<div class="flex col-span-2 row-span-2 h-full w-full rounded-lg bg-white p-4 shadow-md">
  <div>
    <h2 class="mb-2 text-xl font-semibold">City Name</h2>
    <div class="flex">
      <font-awesome-icon  :icon="faUserClock"  class="fa-solid fa-user mt-5 h-12" style="color: #ec5500;"/>
      <p class="mt-4 text-right">
        <span class="ml-6 font-bold text-5xl text-blue-500">126</span>
      </p>
    </div>
  </div>
</div>

<div class="flex h-36 w-full rounded-lg bg-white p-4 shadow-md">
  <div>
    <h2 class="mb-2 text-xl font-semibold">City Name</h2>
    <div class="flex">
      <font-awesome-icon  :icon="faUserTag"  class="fa-solid fa-user mt-5 h-12" style="color: #1e6ecc;"/>
      <p class="mt-4 text-right">
        <span class="ml-6 font-bold text-5xl text-blue-500">126</span>
      </p>
    </div>
  </div>
</div>

<div></div>
<div class="flex h-36 w-full rounded-lg bg-white p-4 shadow-md">
  <div>
    <h2 class="mb-2 text-xl font-semibold">City Name</h2>
    <div class="flex">
      <font-awesome-icon  :icon="faUserGroup"  class="fa-solid fa-user mt-5 h-12" style="color: #ffb800;"/>
      <p class="mt-4 text-right">
        <span class="ml-6 font-bold text-5xl text-blue-500">126</span>
      </p>
    </div>
  </div>
</div>
<div class="flex h-36 w-full rounded-lg bg-white p-4 shadow-md">
  <div>
    <h2 class="mb-2 text-xl font-semibold">City Name</h2>
    <div class="flex">
      <font-awesome-icon  :icon="faUserCheck"  class="fa-solid fa-user mt-5 h-12" style="color: #42ae00;"/>
      <p class="mt-4 text-right">
        <span class="ml-6 font-bold text-5xl text-blue-500">126</span>
      </p>
    </div>
  </div>
</div>
<div class="flex h-36 w-full rounded-lg bg-white p-4 shadow-md">
  <div class="mx-auto">
      <font-awesome-icon  :icon="faCamera"  class="fa-solid fa-user mx-auto mt-5 h-12" style="color: #1e6ecc;"/>
    <h2 class="mb-2 text-md font-semibold">Scan a Registree</h2>
  </div>
</div>
</div>
</div>
<hr class="mt-5 w-3/4 mx-auto shadow" />
<UserTable />
</template>