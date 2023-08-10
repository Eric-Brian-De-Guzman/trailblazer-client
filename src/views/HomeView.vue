<script setup>
import UserTable from '../components/HomeView/UserTable.vue';


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
      <div class="mr-4 text-4xl mt-5 text-blue-500">🏙️</div>
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
      <div class="mr-4 text-4xl mt-5 text-blue-500">🏙️</div>
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
      <div class="mr-4 text-4xl mt-5 text-blue-500">🏙️</div>
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
      <div class="mr-4 text-4xl mt-5 text-blue-500">🏙️</div>
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
      <div class="mr-4 text-4xl mt-5 text-blue-500">🏙️</div>
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
      <div class="mr-4 text-4xl mt-5 text-blue-500">🏙️</div>
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
      <div class="mr-4 text-4xl mt-5 text-blue-500">🏙️</div>
      <p class="mt-4 text-right">
        <span class="ml-6 font-bold text-5xl text-blue-500">126</span>
      </p>
    </div>
  </div>
</div>
</div>
</div>
<hr class="mt-5 w-3/4 mx-auto shadow" />
<UserTable />
</template>