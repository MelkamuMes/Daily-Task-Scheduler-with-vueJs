<script setup>
    import Navbar from '@/components/Navbar.vue';
    import Tasks from '@/components/Task.vue';
    import HomePage from './components/HomePage.vue';
    import AddTask from './components/AddTask.vue';
    import HowToUse from './components/HowToUse.vue';
</script>

<template>
  <Navbar/>
  <HomePage/>
   <Tasks/> 
   <AddTask/>
   <HowToUse/>
</template>

<style >
  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'popins' sans-serif;
  }
 body {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}


</style>