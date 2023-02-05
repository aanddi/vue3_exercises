<script>
export default {
  name: 'App',
  data() {
    return {
      visible1: false,
      visible2: true,
    }
  },

  computed: {
  },
  methods: {
    showItem1: function () {
      this.visible1 = true;
    },

    hideItem2: function () {
      this.visible2 = false;
    }, 

    showItem2: function () {
      this.visible2 = true;
    },
  }
}
</script>

<template>

<p class="box" v-if="visible1">
  Далеко-далеко за словесными горами в стране гласных и согласных живут рыбные тексты. Обеспечивает переписали запятых свою имени журчит рыбными то своих семантика безорфографичный что коварных запятой буквоград строчка над, большого залетают. Журчит.
</p>
<button class="link" @click="showItem1">Показать текст</button>

<br>

<p class="box" v-if="visible2">
  Далеко-далеко за словесными горами в стране гласных и согласных живут рыбные тексты. Обеспечивает переписали запятых свою имени журчит рыбными то своих семантика безорфографичный что коварных запятой буквоград строчка над, большого залетают. Журчит.
</p>
<button class="link" @click="showItem2">Показать текст</button>
<button class="link" @click="hideItem2">Скрыть текст</button>

<br>

<p class="box" v-if="visible2">
  Далеко-далеко за словесными горами в стране гласных и согласных живут рыбные тексты. Обеспечивает переписали запятых свою имени журчит рыбными то своих семантика безорфографичный что коварных запятой буквоград строчка над, большого залетают. Журчит.
</p>
<button class="link" @click="showItem2" v-if="!visible2">Показать текст</button>
<button class="link" @click="hideItem2" v-if="visible2">Скрыть текст</button>

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
