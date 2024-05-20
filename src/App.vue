<template>
  <div class="container">
    <h1 class="head">Counter : {{ counter }}</h1>
    <div class="d-flex">
      <button @click="onIncrement" class="btn btn-success">Add</button>
      <button @click="onReflesh">Reflesh</button>
      <button @click="onDecrement" class="btn btn-danger">Delete</button>
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
<style>
.head {
  text-align: center;
  font-family: "Trebuchet MS", "Lucida Sans Unicode", "Lucida Grande",
    "Lucida Sans", Arial, sans-serif;
}
.d-flex {
  width: 340px;
  text-align: center;
  margin: auto auto;
}
button {
  width: 100px;
  border: 1px solid black;
  padding: 10px;
  border-radius: 20px;
}

button:nth-child(1) {
  background-color: teal;
  font-size: 16px;
  color: white;
}
button:nth-child(2) {
  margin-left: 20px;
  background-color: gold;
  font-size: 16px;
  color: white;
}
button:nth-child(3) {
  margin-left: 20px;
  background-color: red;
  font-size: 16px;
  color: white;
}
</style>
