<template>
  <header>
    <h1>{{ title }}</h1>
    <Button
      @btn-click="$emit('btn-click')"
      :text="showAddTask ? 'Close' : 'Add Task'"
      :color="showAddTask ? 'gray' : 'green'"
    />
  </header>
</template>

<script>
import Button from "./Button.vue";

export default {
  name: "Header",
  props: ["title", "showAddTask"], // one way of registering the props
  //   props: { second way of registering the props
  //     title: String,
  //   },
  //   props: { // one more way of registering the props
  //     title: {
  //       type: String,
  //       required: true,
  //       default: "Todo List",
  //     },
  //   },
  components: { Button },
};
</script>

<style scoped >
header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 20px;
}
</style>