<script>
export default {
  data() {
    return {
      titles: ['Заголовок1', 'Заголовок2', 'Заголовок3'],
    }
  },
  methods: {
    add: function () {
      this.titles.push('Заголовок');
    },
    del: function () {
      this.titles.shift();
    },
    del1: function () {
      this.titles.pop();
    },
    splice: function () {
      this.titles.splice(2, 1);
    },
    sort: function () {
      this.titles.sort();
    },
    reverse: function () {
      this.titles.reverse();
    },
  }
}
</script>

<template>
  <div class="wrapper">
    <ul class="styled">
      <li v-for="elem in titles" class="box">{{ elem }}</li>
    </ul>
    <button class="link" @click="add">Добавить заголовок</button>
    <button class="link" @click="del">Удалить заголовок первый пункт</button>
    <button class="link" @click="del1">Удалить заголовок последний пункт</button>
    <button class="link" @click="splice">Удалить заголовок предпоследний пункт</button>
    <button class="link" @click="sort">Отсортировать</button>
    <button class="link" @click="reverse">Выставить в обратном порядке</button>
  </div>

</template>

<style>
.wrapper {
  text-align: center;
  margin: 0 auto;
  width: 400px;
}

.link {
  color: #ffffff;
  background: #02bd02;
  font-weight: bold;
  font-size: 20px;
  padding: 5px 20px;
  transition: all 0.3s ease-out;
  margin-top: 20px;
  width: 100%;
}

.link:hover {
  background-color: #b60046;
  color: #0e0101;
}

.box {
  width: 300px;
  padding: 20px 10px;
  border: 1px solid #000;
  background-color: #fff;
  margin: 10px auto;
  width: 100%;
}
</style>