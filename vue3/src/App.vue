<script>
export default {
  name: 'App',
  data() {
    return {
      num: 5,
      num1: 1,
      num2: 2,
      num3: 3,
    }
  }
}
</script>

<template>

  <div class="box"> Квадрат числа num(5) равен {{ num * num }} </div>
  <div class="box"> Сумма чисел num1(1), num2(2), num3(3)  равна {{ num1 + num2 + num3 }} </div>

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
