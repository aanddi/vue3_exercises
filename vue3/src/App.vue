<script>
export default {
  name: 'App',
  data() {
    return {
      visible: true,
    }
  },
  computed: {
  },
  methods: {
    btn: function () {
      this.visible = !this.visible;
    }
  }
}
</script>

<template>

  <div class="wrapper" v-show="visible">
    <p class="box">
      Далеко-далеко за словесными горами в стране гласных и согласных живут рыбные тексты. Инициал
      ведущими, образ дал букв пор рукописи то буквенных своих путь всемогущая, проектах грамматики переулка
      реторический курсивных текстами власти.
    </p>
    <p class="box">
      Далеко-далеко за словесными горами в стране гласных и согласных живут рыбные тексты. Инициал
      ведущими, образ дал букв пор рукописи то буквенных своих путь всемогущая, проектах грамматики переулка
      реторический курсивных текстами власти.
    </p>
    <p class="box">
      Далеко-далеко за словесными горами в стране гласных и согласных живут рыбные тексты. Инициал
      ведущими, образ дал букв пор рукописи то буквенных своих путь всемогущая, проектах грамматики переулка
      реторический курсивных текстами власти.
    </p>
  </div>
  <button class="link" @click="btn">{{ visible ? 'Скрыть' : 'Показать' }}</button>

</template>

<style>
body {
  margin: 30px;
}
.link {
  color: #050505;
  background: #02bd02;
  font-weight: bold;
  font-size: 20px;
  padding: 10px 40px;
  border-radius: 40px;
  transition: all 0.3s ease-out;
  margin: 20px;
  display: block;
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
  margin: 10px;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: row;
}
.wrapper {
  padding: 20px 30px;
  border: 1px solid #000;
  display: flex;
  width: 1000px;
  background: #2dec07;
}
</style>