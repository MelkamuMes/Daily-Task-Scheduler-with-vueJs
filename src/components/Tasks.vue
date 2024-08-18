<script setup>
console.log('Before import');
import taskData from '../TaskLists.json';
console.log('After import, data:', taskData)
import Task from './Task.vue'
import {ref} from 'vue'

const tasks = ref(taskData);
console.log(tasks.value)
</script> 

<template>
   <section class="job-section">
      <div class="container">
         <h2 class="section-title">Browse tasks</h2>
      <div class="job-grid">
            <Task />
      </div>
      </div>
  </section>

      <!-- <Task v-for="Task in Tasks" :key="Task.id" :Task="Task"/> -->
</template>

<style>

.job-section {
  background-color: #ebf8ff; /* equivalent to bg-blue-50 */
  padding: 2.5rem 1rem; /* equivalent to px-4 py-10 */
}

.container {
  max-width: 1140px; /* equivalent to container-xl */
  margin: auto;
}

.section-title {
  font-size: 1.875rem; /* equivalent to text-3xl */
  font-weight: bold; /* equivalent to font-bold */
  color: #442626; /* equivalent to text-green-500 */
  margin-bottom: 1.5rem; /* equivalent to mb-6 */
  text-align: center;
}

.job-grid {
  display: grid;
  grid-template-columns: repeat(1, 1fr); /* equivalent to grid-cols-1 */
  gap: 1.5rem; /* equivalent to gap-6 */
}

@media (min-width: 768px) {
  .job-grid {
    grid-template-columns: repeat(3, 1fr); /* equivalent to md:grid-cols-3 */
  }
}

</style>