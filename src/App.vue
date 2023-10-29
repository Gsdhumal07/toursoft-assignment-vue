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
          title: "Decide the destination",
          completed: true,
        },
        {
          id: 2,
          title: "Do the Bookings",
          completed: true,
        },
        {
          id: 3,
          title: "Check the details",
          completed: false,
        },
        {
          id: 4,
          title: "Go through the local guides",
          completed: false,
        },
        {
          id: 5,
          title: "Enjoy the journey",
          completed: false,
        },
      ],
    };
  },
};
</script>