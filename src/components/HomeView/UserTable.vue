<template>
  <div class="p-4 mx-auto w-3/4">
    <h2 class=" mb-4 text-4xl font-medium">Users</h2>
    <table class="table-auto w-full">
      <thead>
        <tr>
          <th class="px-4 py-2">FULL NAME</th>
          <th class="px-4 py-2">COMPANY</th>
          <th class="px-4 py-2">EMAIL ADDRESS</th>
          <th class="px-4 py-2">CONTACT NUMBER</th>
          <th class="px-4 py-2">DATE REGISTERED</th>
          <th class="px-4 py-2">STATUS</th>
        </tr>
      </thead>
      <tbody>
        <tr v-for="(person, index) in people" :key="index">
          <td class="border px-4 py-2">{{ person.name }}</td>
          <td class="border px-4 py-2">{{ person.age }}</td>
          <td class="border px-4 py-2">{{ person.location }}</td>
          <td class="border px-4 py-2">{{ person.location }}</td>
          <td class="border px-4 py-2">{{ person.location }}</td>
          <td class="border px-4 py-2">{{ person.location }}</td>
          
        </tr>
      </tbody>
    </table>
  </div>
</template>

<script>
export default {
  data() {
    return {
      people: [
        { name: 'John Doe', age: 30, location: 'New York' },
        { name: 'Jane Smith', age: 25, location: 'Los Angeles' },
        { name: 'Alice Johnson', age: 28, location: 'Chicago' },
        { name: 'Bob Brown', age: 22, location: 'San Francisco' },
      ],
    };
  },
};
</script>

