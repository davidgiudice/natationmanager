<template>
  <div class="bg-white shadow-md rounded p-4 mt-4">
    <h2 class="text-xl font-semibold mb-4">Attendees</h2>
    <ul>
      <li v-for="attendee in attendees" :key="attendee.id" class="mb-2">
        {{ attendee.name }}
      </li>
    </ul>
  </div>
</template>

<script setup>
import { ref } from 'vue';

const attendees = ref([
  { id: 1, name: 'John Doe' },
  { id: 2, name: 'Jane Smith' },
]);
</script>