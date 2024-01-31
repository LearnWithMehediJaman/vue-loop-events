<script setup>
const persons = [
  {
    'name': 'John Doe',
    'age': 30,
    'city': 'New York'
  },

  {
    'name': 'Jimmy Doe',
    'age': 30,
    'city': 'New York'
  },

  {
    'name': 'Jane Doe',
    'age': 30,
    'city': 'New York'
  },

  {
    'name': 'Jackie Doe',
    'age': 30,
    'city': 'New York'
  },

  {
    'name': 'Jenny Doe',
    'age': 30,
    'city': 'New York'
  },

  {
    'name': 'Jenny Doe',
    'age': 30,
    'city': 'New York'
  }
];

</script>

<template>
  <table class="table-auto w-1/2 mt-4 ml-5 bg-blue-300 ">
    <thead>
      <th class="border border-slate-500 p-2">Name</th>
      <th class="border border-slate-500 p-2">Age</th>
      <th class="border border-slate-500 p-2">Location</th>
    </thead>

    <tbody>
      <tr v-for="(person, index) in persons" :key="index">
        <td class="border border-slate-500 text-center p-2">{{ person.name }}</td>
        <td class="border border-slate-500 text-center p-2">{{ person.age }}</td>
        <td class="border border-slate-500 text-center p-2">{{ person.city }}</td>
      </tr>
    </tbody>
  </table>
</template>
