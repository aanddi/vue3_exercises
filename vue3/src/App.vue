<script>
export default {
  data() {
    return {
      obj: {
        block: true,
        selected: false,
      },
    }
  },
  methods: {
  }
}
</script>

<template>
  <p :class="obj">
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

.selected {
  background-color: red;
  color: #fff;
}

</style>