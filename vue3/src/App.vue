<script>
export default {
  name: 'App',
  data() {
    return {
      age: prompt('Введите свой возвраст')
    }
  },

  computed: {
  },

  methods: {
  }
}
</script>

<template>

  <div class="box" v-if="age < 18">Подросток</div>
  <div class="box" v-else-if="19 < age && age < 25">Молодой человек</div>
  <div class="box" v-else-if="age > 26">Мужчина</div>

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
  margin: 10px;
  display: flex;
  align-items: center;
  justify-content: center;

}
</style>
