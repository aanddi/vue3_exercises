<script>
export default {
  name: 'App',
  data() {
    return {
      day: new Date().getDay(),
    }
  },

  computed: {
  },

  methods: {
  }
}
</script>

<template>

  <p class="box" v-if="day == '1'">Понедельник</p>
  <p class="box" v-if="day == '2'">Вторник</p>
  <p class="box" v-if="day == '3'">Среда</p>
  <p class="box" v-if="day == '4'">Четверг</p>
  <p class="box" v-if="day == '5'">Пятница</p>
  <p class="box" v-if="day == '6'">Суббота</p>
  <p class="box" v-if="day == '7'">Воскресенье</p>

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
