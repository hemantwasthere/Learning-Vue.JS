<template>
  <header>
    <h1>{{ title }}</h1>
    <Button text="Add Task" color="green" />
  </header>
</template>

<script>
import Button from "./Button.vue";

export default {
  props: ["title"], // one way of registering the props
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