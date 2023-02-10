<script>
export default {
  name: 'App',
  data() {
    return {
      isAdmin: true,
    }
  },

  computed: {

  },

  methods: {
    log: function () {
      this.isAdmin = !this.isAdmin;
    }
  }
}
</script>

<template>

  <button class="link" @click="log">{{ isAdmin ? 'Выйти' : 'Войти' }}</button>

  <p class="box" v-if="isAdmin">
    Далеко-далеко за словесными горами в стране гласных и согласных живут рыбные тексты.
    Реторический маленький дал, повстречался лучше агентство толку рукопись? Всемогущая сих, одна курсивных свою
    возвращайся вопроса ведущими дал. Большого, дороге все.
  </p>

  <p class="box" v-else>Войдите в свою учетную запись</p>
  
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
  width: 500px;
  padding: 20px;
  border: 1px solid #000;
  margin: 10px;

}
</style>
