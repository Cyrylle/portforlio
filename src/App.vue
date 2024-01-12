<template>
  <div id="app">
    <router-view/>
    <!-- <TaskManager /> -->
  </div>
</template>

<script>
import TaskManager from "@/views/TaskManager.vue";

export default {
  components: {
    TaskManager,
  },
};
</script>

<style>
/* Add your global styles here if needed */
</style>
