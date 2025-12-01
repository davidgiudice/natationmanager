<template>
  <div class="border p-2 rounded shadow-sm flex justify-between items-center">
    <div>
      <h3 class="font-bold text-lg">{{ course.name }}</h3>
      <p class="text-sm text-gray-600">Attendees: {{ course.attendees }}</p>
    </div>
    <button class="bg-blue-500 text-white rounded px-2 py-1">View</button>
  </div>
</template>

<script setup>
import { defineProps } from 'vue';

const props = defineProps({
  course: Object,
});
</script>