<template>
  <button @click="addTask" class="btn" :style="{ backgroundColor: color }">
    {{ text }}
  </button>
</template>

<script>
export default {
  name: "Button",
  props: ["text", "color"],
  methods: {
    addTask() {
      this.$emit('show-add-task')
    },
  },
};
</script>