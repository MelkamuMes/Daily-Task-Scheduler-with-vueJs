<script setup>
import HomeItem from './HomeItem.vue';
</script>

<template>
  <!-- Daily and Prior -->
  <section class="section">
    <div class="container">
      <div class="grid">
        <Card class="card-green">
          <h2 class="card-title">Daily Task Scedule</h2>
          <p class="card-text">
            Daily tasks are routine or scheduled activities that need to be completed within the day. These tasks are usually time-sensitive and help in managing day-to-day responsibilities. They can range from work-related duties to personal errands.
          </p>
          <a
            href="#SeeTask"
            class="button"
          >
            See Task
          </a>
        </Card>
        <Card class="card-green">
          <h2 class="card-title">Your Prior Time Sdhedule</h2>
          <p class="card-text">
            Prior tasks are tasks that have been carried over from previous days and still need attention. These may include unfinished tasks or important items that have been rescheduled. Prior tasks often have higher priority due to their pending status.
          </p>
          <a
            href="#AddTask"
            class="button button-green"
          >
            Add Job
          </a>
        </Card>
      </div>
    </div>
  </section>
</template>

<style>
/* Section Styles */
.section {
  padding: 1rem 0;
}

/* Container Styles */
.container {
  max-width: 1140px;
  margin: auto;
}

/* Grid Layout */
.grid {
  display: grid;
  grid-template-columns: 1fr;
  gap: 1rem;
  padding: 1rem;
  border-radius: 0.5rem;
}

@media (min-width: 768px) {
  .grid {
    grid-template-columns: 1fr 1fr;
  }
}

/* Card Styles */
.card-title {
  font-size: 1.5rem;
  font-weight: bold;
}

.card-text {
  margin-top: 0.5rem;
  margin-bottom: 1rem;
}

/* Button Styles */
.button {
  display: inline-block;
  background-color: rgb(77, 44, 44);
  color: white;
  border-radius: 0.5rem;
  padding: 0.5rem 1rem;
  text-decoration: none;
  transition: background-color 0.3s;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
}

.button:hover {
  background-color: #4e2f2f;
}

/* Green Card and Button Styles */
.card-green {
  background-color: #8b5e5e9f;
  padding: 40px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
}

.button-green {
  background-color: #553232;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
}

.button-green:hover {
  background-color: #503232;
}






/* test */
.card {
  padding: 1.5rem; /* Equivalent to p-6 */
  border-radius: 1rem; /* Equivalent to rounded-lg */
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1); /* Equivalent to shadow-md */
}

/* Default Background Color */
.bg-gray-100 {
  background-color: #f7fafc; /* Equivalent to bg-gray-100 */
}

/* Additional Background Classes */
.bg-white {
  background-color: white;
}

.bg-blue-100 {
  background-color: #ebf8ff;
}

.bg-green-100 {
  background-color: #634040;
}
</style>
