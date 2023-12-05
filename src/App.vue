<template>
  <div id="app">
    <task v-bind:tasks="tasks"></task>
  </div>
</template>

<script>
import Task from "./components/Task";

export default {
  name: "App",
  components: {
    Task,
  },
  data() {
    return {
      tasks: [
        {
          id: 1,
          title: "Learn Vue router",
          completed: true,
        },
        {
          id: 2,
          title: "Send cold Email",
          completed: true,
        },
        {
          id: 3,
          title: "Lunch",
          completed: false,
        },
        {
          id: 4,
          title: "Go shopping",
          completed: false,
        },
        {
          id: 5,
          title: "Make Dinner",
          completed: false,
        },
      ],
    };
  },
};
</script>