<script>
export default {
  name: 'App',
  data() {
    return {
      visible1: true,
      visible2: true,
      visible3: true,
    }
  },

  computed: {
  },

  methods: {
    toggle1: function () {
      this.visible1 =  !this.visible1;
    },
    toggle2: function () {
      this.visible2=  !this.visible2;
    },
    toggle3: function () {
      this.visible3 =  !this.visible3;
    }

  }
}
</script>

<template>

<p class="box" v-if="visible1">
  Далеко-далеко за словесными горами в стране гласных и согласных живут рыбные тексты. Обеспечивает переписали запятых свою имени журчит рыбными то своих семантика безорфографичный что коварных запятой буквоград строчка над, большого залетают. Журчит.
</p>
<button class="link" @click="toggle1">{{visible1}}</button>

<p class="box" v-if="visible2">
  Далеко-далеко за словесными горами в стране гласных и согласных живут рыбные тексты. Обеспечивает переписали запятых свою имени журчит рыбными то своих семантика безорфографичный что коварных запятой буквоград строчка над, большого залетают. Журчит.
</p>
<button class="link" @click="toggle2">{{visible2}}</button>

<p class="box" v-if="visible3">
  Далеко-далеко за словесными горами в стране гласных и согласных живут рыбные тексты. Обеспечивает переписали запятых свою имени журчит рыбными то своих семантика безорфографичный что коварных запятой буквоград строчка над, большого залетают. Журчит.
</p>
<button class="link" @click="toggle3">{{visible3}}</button>


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
