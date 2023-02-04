<script>
export default {
  name: 'App',
}
</script>

<template>
  <div class="wrapper">
    <div class="box">
      <h3 class="title">Title</h3>
      <p class="sub-title">
        Далеко-далеко за словесными, горами в стране гласных и согласных живут рыбные тексты.
        Грустный его за вопрос прямо, заголовок раз моей переписали продолжил.
        Над парадигматическая рукописи до грустный предупреждал последний свою то залетают!
      </p>
    </div>
    <div class="box">
      <h3 class="title">Title</h3>
      <p class="sub-title">
        Далеко-далеко за словесными, горами в стране гласных и согласных живут рыбные тексты.
        Грустный его за вопрос прямо, заголовок раз моей переписали продолжил.
        Над парадигматическая рукописи до грустный предупреждал последний свою то залетают!
      </p>
    </div>
    <div class="box">
      <h3 class="title">Title</h3>
      <p class="sub-title">
        Далеко-далеко за словесными, горами в стране гласных и согласных живут рыбные тексты.
        Грустный его за вопрос прямо, заголовок раз моей переписали продолжил.
        Над парадигматическая рукописи до грустный предупреждал последний свою то залетают!
      </p>
    </div>
  </div>
</template>

<style>
body {
  margin: 30px;
  font-family: Arial, Helvetica, sans-serif;
}

.wrapper {
  display: flex;
}

.box {
  width: 300px;
  border: 1px solid black;
  border-radius: 30px;
  color: #fff;
  background-color: #000;
  padding: 30px;
  margin: 10px
}

.box:hover {
  background-color: #fff;
  color: #000;
}

.title {
  font-size: 30px;
  text-align: center;
}

.sub-title {
  text-align: justify;
}
</style>
