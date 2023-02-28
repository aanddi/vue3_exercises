<script>
export default {
  props: {
    name: String,
    salary: Number,
    age: Number
  },
  data() {
    return {
    }
  }
}
</script>

<template>
  <div class="block">
    <h1>{{ name }}</h1>
    <h1>{{ salary }}</h1>
    <h1>{{ age }}</h1>
  </div>
</template>


<style>
.block {
  border: 1px solid black;
  padding: 20px;
  margin: 50px;
  width: 300px;
}
</style>