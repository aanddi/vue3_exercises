<script>
export default {
  data() {
    return {
      obj: {
        block: true,
        red: false,
      },
      obj1: {
        block: true,
        toggle: false,
      },
    }
  },
  methods: {
    setRed: function () {
      this.obj.red = !this.obj.red;
    },
    toggle: function () {
      this.obj1.toggle = !this.obj1.toggle;
    }
  }
}
</script>

<template>
  <p :class="obj">
    Далеко-далеко за словесными горами в стране гласных и согласных живут рыбные тексты. Вопроса заголовок, он рукопись
    маленький за предупредила журчит путь образ сбить лучше! Текст реторический, большой она жаренные lorem напоивший от
    всех.
  </p>
  <button class="btn" @click="setRed">{{obj.red}}</button>

  <p :class="obj1">
    Далеко-далеко за словесными горами в стране гласных и согласных живут рыбные тексты. Вопроса заголовок, он рукопись
    маленький за предупредила журчит путь образ сбить лучше! Текст реторический, большой она жаренные lorem напоивший от
    всех.
  </p>
  <button class="btn" @click="toggle">{{obj1.toggle}}</button>
</template>

<style>
.block {
  border: 1px solid black;
  padding: 20px;
  width: 300px;
  margin: 20px;
  text-align: justify;
}

.red {
  background-color: red;
  color: #fff;
}

.btn {
  background-color: #d80808;
  color: #fff;
  padding: 15px;
  margin-left: 100px;
  border-radius: 10px;
}

.toggle {
  display: none;
}

</style>