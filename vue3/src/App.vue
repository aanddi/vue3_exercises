<script>
export default {
  name: 'App',
  data() {
    return {
      num: 0,
    }
  },
  methods: {

    getNumber: function (num) {
      this.num  = prompt(num);
      return this.num;
    },

    showNumber: function () {
      return this.num;
    },

    square: function() {
      return alert(this.num ** 2);
    },

    cube: function () {
      return alert(this.num ** 3);
    },

  }
}
</script>

<template>

<div class="box">Число: {{ getNumber() }}</div>

<button @click="square" class="link">Возведение {{ showNumber() }} в квадрат</button>
<button @click="cube" class="link">Возведение {{ showNumber() }} в куб</button>

</template>

<style>

body {
  margin: 60px;
  font-family: Arial, Helvetica, sans-serif;
}

.box {
  background-color: #fc251e;
  display: inline-block;
  padding: 10px 40px;
  border-radius: 40px;
  font-weight: bold;
  margin: 20px;
}


.link {
  background: red;
  font-weight: bold;
  font-size: 20px;
  padding: 20px 30px;
  border-radius: 40px;
  transition: all 0.3s ease-out;
  margin: 20px;
}

.link:hover {
  background-color: #000;
  color: red;
}
</style>
