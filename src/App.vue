<template>
  <div class="min-h-screen bg-gray-100">
    <header class="bg-blue-600 text-white py-4">
      <h1 class="text-center text-2xl font-bold">Natation Manager</h1>
    </header>
    <main class="p-4">
      <CourseList />
    </main>
  </div>
</template>

<script setup>
import CourseList from './components/CourseList.vue';
</script>

<style scoped>
</style>