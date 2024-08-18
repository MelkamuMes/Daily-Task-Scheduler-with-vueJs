<template>
    <div class="form-container" id="AddTask">
      <h3 class="form-title">Add Task</h3>
      <form @submit.prevent="handleSubmit">
        <div class="form-group">
          <label for="title">Task Title</label>
          <input type="text" id="title" v-model="task.title" required />
        </div>
  
        <div class="form-group">
          <label for="datetime">Date & Time</label>
          <input type="datetime-local" id="datetime" v-model="task.datetime" required />
        </div>
  
        <div class="form-group">
          <label for="description">Description</label>
          <textarea id="description" v-model="task.description" required></textarea>
        </div>
  
        <div class="form-group">
          <label for="priority">Priority</label>
          <select id="priority" v-model="task.priority" required>
            <option value="High">High</option>
            <option value="Medium">Medium</option>
            <option value="Low">Low</option>
          </select>
        </div>
  
        <button type="submit" class="submit-button">Add Task</button>
      </form>
    </div>
  </template>
  
  <script setup>
  import { ref } from 'vue';
  
  const task = ref({
    title: '',
    datetime: '',
    description: '',
    priority: 'Medium',
  });
  
  const handleSubmit = () => {
    console.log('Task submitted:', task.value);
    // You can add your form submission logic here.
  };
  </script>
  
  <style>
  .form-container {
    max-width: 800px;
    margin: 2rem auto;
    padding: 2rem;
    background-color: #d4bebe;
    border-radius: 8px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  }
  
  .form-title {
    font-size: 1.5rem;
    font-weight: bold;
    text-align: center;
    margin-bottom: 1.5rem;
    color: #333;
  }
  
  .form-group {
    margin-bottom: 1rem;
  }
  
  .form-group label {
    display: block;
    margin-bottom: 0.5rem;
    font-weight: bold;
    color: #333;
  }
  
  .form-group input,
  .form-group textarea,
  .form-group select {
    width: 100%;
    padding: 0.5rem;
    font-size: 1rem;
    border: 1px solid #ccc;
    border-radius: 4px;
  }
  
  .form-group textarea {
    height: 100px;
    resize: vertical;
  }
  
  .submit-button {
    width: 100%;
    padding: 0.75rem;
    font-size: 1rem;
    font-weight: bold;
    background-color: #472a2a;
    color: white;
    border: none;
    border-radius: 4px;
    cursor: pointer;
    transition: background-color 0.3s ease;
  }
  
  .submit-button:hover {
    background-color: #6e4141;
  }
  </style>
  