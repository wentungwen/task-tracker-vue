<template>
  <header>
    <h1>{{ title }}</h1>
    <Button text="add task" color="green" />
  </header>
</template>
<script>
import Button from "./Button";
export default {
  name: "header",
  props: {
    title: {
      type: String,
      default: "hello!!",
    },
  },
  components: {
    Button,
  },
};
</script>
<style scoped>
header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 20px;
}
</style>
