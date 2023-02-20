<script>
export default {
  data() {
    return {
      isValid: true,
      isDisabled: false,
    }
  },
  methods: {

  }
}
</script>

<template>
  <p :class="{block: isValid, color: isValid, bg: isValid}">
    Далеко-далеко за словесными горами в стране гласных и согласных живут рыбные тексты. Вопроса заголовок, он рукопись
    маленький за предупредила журчит путь образ сбить лучше! Текст реторический, большой она жаренные lorem напоивший от
    всех.
  </p>

  <p :class="{block: isValid, bold: isValid, cursive: isValid }">
    Далеко-далеко за словесными горами в стране гласных и согласных живут рыбные тексты. Вопроса заголовок, он рукопись
    маленький за предупредила журчит путь образ сбить лучше! Текст реторический, большой она жаренные lorem напоивший от
    всех.
  </p>
</template>

<style>
.block {
  border: 1px solid black;
  padding: 20px;
  width: 300px;
  margin: 20px;
  text-align: justify;
}

.color.bg {
  color: green;
  background-color: yellow;
}

.bold.cursive {
  font-weight: bold;
  font-style: italic;
}
</style>