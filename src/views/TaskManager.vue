<template>
  <div id="app" class="container mt-5">
    <h1>Name List</h1>
    <form @submit.prevent="addTask">
      <div class="form-group">
        <label for="taskInput">Name:</label>
        <input
          type="text"
          class="form-control"
          id="taskInput"
          v-model="newTask"
          required
        />
      </div>
      <button type="submit" class="btn border btn-primary:hover ">Add Name</button>
    </form>
    <ul class="list-group mt-3">
      <li
        v-for="(task, index) in tasks"
        :key="index"
        class="list-group-item"
      >
        {{ task }}
        <button @click="editTask(index)" class="btn btn-sm btn-warning ml-2">Edit</button>
        <button @click="deleteTask(index)" class="btn btn-sm btn-danger ml-2">Delete</button>
      </li>
    </ul>
  </div>
</template>

<script>
const pageTitle = 'TaskManager'
export default {
  data() {
    return {
      newTask: "",
      tasks: [],
    };
  },
  methods: {
    addTask() {
      if (this.newTask.trim() !== "") {
        this.tasks.push(this.newTask.trim());
        this.newTask = "";
      }
    },
    editTask(index) {
      const updatedTask = prompt("Edit Task:", this.tasks[index]);
      if (updatedTask !== null) {
        this.$set(this.tasks, index, updatedTask.trim());
      }
    },
    deleteTask(index) {
      const confirmDelete = confirm("Are you sure you want to delete this task?");
      if (confirmDelete) {
        this.tasks.splice(index, 1);
      }
    },
  },
};
</script>

<style>




.container {
  background-color: #4ca4ec;
  padding: 20px;
  border-radius: 8px;
  box-shadow: 0 0 20px rgba(0, 0, 0, 0.1);
}

h1 {
  color: #e90b0b;
  text-align: center;
  font-weight: bold;
}

.form-group {
  margin-bottom: 20px;
}

.form-control {
  width: 100%;
  padding: 12px;
  font-size: 16px;
  border: 1px solid #B0BEC5;
  border-radius: 4px;
  background-color: #ececf1;
  color: #37474F;
}

.btn-primary {
  background-color: #1976D2;
  color: #fff;
  font-size: 16px;
  padding: 12px 20px;
  border: none;
  border-radius: 4px;
  cursor: pointer;
}

.list-group-item {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-top: 15px;
  padding: 15px;
  border: 1px solid #B0BEC5;
  border-radius: 8px;
  background-color: #fff;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
}

.btn-warning,
.btn-danger {
  padding: 8px 12px;
  border: none;
  border-radius: 4px;
  cursor: pointer;
}

.btn-warning {
  background-color: #FFA000;
  color: #212529;
}

.btn-danger {
  background-color: #E53935;
  color: #fff;
}



</style>



