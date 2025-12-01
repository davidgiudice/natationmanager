<template>
  <div class="bg-white shadow-md rounded p-4">
    <h2 class="text-xl font-semibold mb-4">Courses</h2>
    <ul>
      <li v-for="course in courses" :key="course.id" class="mb-2">
        <CourseCard :course="course" />
      </li>
    </ul>
  </div>
</template>

<script setup>
import { ref } from 'vue';
import CourseCard from './CourseCard.vue';

const courses = ref([
  { id: 1, name: 'Swimming Basics', attendees: 10 },
  { id: 2, name: 'Advanced Techniques', attendees: 8 },
]);
</script>