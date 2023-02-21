<script>
export default {
  data() {
    return {
      num: 0,
      num1: 0,
      num2: 0,
      result: 0,
      result1: 0,
      text1: 'hello',
      text2: 'world',
      fullName: '',
      name: '',
      surname: '',
      patronymic: '',
    }
  },
  methods: {
    calc: function () {
      this.result = this.num ** 2
    },
    calc1: function () {
      this.result1 = Number(this.num1) + Number(this.num2);
    },

    calc2: function () {
      const a = this.text1;
      this.text1 = this.text2;
      this.text2 = a;
    },
    user: function () {
      const user = this.fullName.split(' ');
      this.surname = user[0];
      this.name = user[1];
      this.patronymic = user[2];
    },
  }
}
</script>

<template>
  <div class="wrapper">
    <div class="block">
      <p>{{ result }}</p>
      <input class="block_input" v-model="num">
      <button class="btn" @click="calc">Посчитать квадрат</button>
    </div>

    <div class="block">
      <p>{{ result1 }}</p>
      <input class="block_input" v-model="num1">
      <input class="block_input" v-model="num2">
      <button class="btn" @click="calc1">Посчитать сумму</button>
    </div>

    <div class="block">
      <input class="block_input" v-model="text1">
      <input class="block_input" v-model="text2">
      <button class="btn" @click="calc2">Поменять</button>
    </div>

    <div class="block">
      <input class="block_input" v-model="fullName">
      <p><span>Фамилия: </span>{{ surname }}</p>
      <p><span>Имя: </span>{{ name }}</p>
      <p><span>Отчество: </span>{{ patronymic }}</p>
      <button class="btn" @click="user">Кнопка</button>
    </div>
  </div>
</template>

<style>
.wrapper {
  display: flex;
  justify-content: space-around;
}
.block {
  border: 1px solid black;
  padding: 20px;
  width: 300px;
  margin: 20px 30px;
  text-align: justify;
  display: flex;
  justify-content: center;
  flex-direction: column;
  align-items: center;
}

.block_input {
  width: 200px;
  margin: 10px 10px;
  padding: 5px;
  border: 1px solid black;
  border-radius: 10px;
}

.btn {
  background-color: #fd0606;
  padding: 10px;
  border-radius: 10px;
  border: 1px solid #fd0606;
  transition: all 0.4s ease-out;
  margin-top: 10px;
}

.btn:hover {
  background-color: #fff;
  color: #fd0606;
  border: 1px solid #fd0606;
}

p {
  color: #fd0606;
  padding: 5px;
}

span {
  color: #000;
  font-weight: bold;
}
</style>