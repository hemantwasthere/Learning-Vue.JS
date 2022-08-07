<template>
  <h3>
    {{task.text}}
    {{task.done}}
  </h3>
</template>

<script>
export default {
  name: "Task",
  props: {
    task: Object,
  },
};
</script>