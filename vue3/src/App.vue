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

  }
}
</script>

<template>

<p class="box" v-if="visible">
  Далеко-далеко за словесными горами в стране гласных и согласных живут рыбные тексты. Обеспечивает переписали запятых свою имени журчит рыбными то своих семантика безорфографичный что коварных запятой буквоград строчка над, большого залетают. Журчит.
</p>

<p class="box" v-if="!visible">
  Далеко-далеко за словесными горами в стране гласных и согласных живут рыбные тексты. Обеспечивает переписали запятых свою имени журчит рыбными то своих семантика безорфографичный что коварных запятой буквоград строчка над, большого залетают. Журчит.
</p>

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
