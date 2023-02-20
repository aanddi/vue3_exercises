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
  <p :class="{ active: isValid, valid: isDisabled, block: isValid }">
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

.active {
  display: block;
}
</style>