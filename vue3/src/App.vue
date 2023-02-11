<script>
export default {
  name: 'App',
  data() {
    return {
    }
  },
  computed: {
  },
  methods: {

  }
}
</script>

<template>
  <div class="wrapper">
    <div class="box" v-for="num in 30">
      <h1 class="title">{{ num }}</h1>
      <p>
        Далеко-далеко за словесными горами в стране гласных и согласных живут рыбные тексты. Журчит ты реторический
        строчка безорфографичный скатился взгляд заголовок лучше встретил алфавит букв, до предупредила о, подпоясал над
        которое если щеке.
      </p>
    </div>
  </div>



</template>

<style>
.box {
  width: 300px;
  padding: 15px 10px;
  border: 1px solid #000;
  background-color: #fff;
  margin: 10px;
  text-align: justify;
  display: flex;
  flex-direction: column;
  align-items: center;
}

.wrapper {
display: flex;
flex-wrap: wrap;
justify-content: center;
}

.title {
  font-weight: bold;
  font-size: 30px;
}
</style>