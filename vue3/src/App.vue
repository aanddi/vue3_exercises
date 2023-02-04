<script>
export default {
  name: 'App',
  data() {
    return {
      arr: ['x', 'y', 'z'],
      arr1: [1, 2, 3],
    }
  }
}
</script>

<template>
  <!-------------- №1 -----------------> <br><hr><br>
  <p class="box"> {{ arr[0] }} </p>
  <p class="box"> {{ arr[1] }} </p>
  <p class="box"> {{ arr[2] }} </p>

  <!-------------- №2 -----------------> <br><hr><br>
  <p class="box"> {{ arr1[0] + arr1[1] + arr1[2] }} </p>


</template>

<style>
body {
  margin: 60px;
  font-family: Arial, Helvetica, sans-serif;
}

.box {
  background-color: #d39b00;
  display: inline-block;
  padding: 20px 60px;
  border-radius: 40px;
  font-weight: bold;
  margin: 30px;
}

/*
.link {
  background: red;
  font-weight: bold;
  font-size: 20px;
  padding: 20px 50px;
  border-radius: 40px;
  transition: all 0.3s ease-out;
}

.link:hover {
  background-color: #000;
  color: red;
}
*/
</style>
