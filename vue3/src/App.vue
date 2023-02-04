<script>
export default {
  name: 'App',
  data() {
    return {
      name: 'Andrey',
      lastname: 'Kuropatkin',
      age: 19,
    }
  }
}
</script>

<template>

  <div class="box">{{ name }}</div>
  <div class="box">{{ lastname }}</div>
  <div class="box">{{ age }}</div>
  
</template>

<style>

body {
  margin: 30px;
  font-family: Arial, Helvetica, sans-serif;
}

.wrapper {
  display: flex;
}

.box {
  display: inline-block;
  border: 1px solid black;
  border-radius: 30px;
  color: #fff;
  background-color: #000;
  padding: 30px;
  margin: 10px
}

.box:hover {
  background-color: #fff;
  color: #000;
}

</style>
