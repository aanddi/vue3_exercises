<script>
export default {
  name: 'App',
  data() {
    return {
    }
  },
  methods: {
		date: function() {
      alert(new Date().toLocaleDateString())
    }
	}
}
</script>

<template>

  <!-------------- №1 -----------------> <br><hr><br>
  <button @click="date" class="link">Нажми, чтобы узнать текущую дату</button>

  <!-------------- №2 -----------------> <br><hr><br>
  <button @mouseover="date" class="link">Наведи, чтобы узнать текущую дату</button>

</template>

<style>
body {
  margin: 60px;
  font-family: Arial, Helvetica, sans-serif;
}

.box {
  background-color: #fc251e;
  display: inline-block;
  padding: 10px 40px;
  border-radius: 40px;
  font-weight: bold;
}


.link {
  background: red;
  font-weight: bold;
  font-size: 20px;
  padding: 20px 30px;
  border-radius: 40px;
  transition: all 0.3s ease-out;
}

.link:hover {
  background-color: #000;
  color: red;
}

</style>
