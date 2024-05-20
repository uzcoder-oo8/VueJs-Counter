<template>
  <div class="container">
    <h1>Counter : {{ counter }}</h1>
    <div class="d-flex">
      <button @click="onIncrement" class="btn btn-success">Add</button>
      <button @click="onReflesh">Reflesh</button>
      <button @click="onDecrement" class="btn btn-danger ml-">Delete</button>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      counter: 0,
    };
  },
  methods: {
    onIncrement() {
      this.counter += 1;
    },
    onDecrement() {
      this.counter -= 1;
    },
    onReflesh() {
      this.counter = 0;
    },
  },
};
</script>
<style></style>
