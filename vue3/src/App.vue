<script>
export default {
  name: 'App',
  data() {
    return {
      text: 'Абзац',
    }
  },
  methods: {

    task2: function () {
      this.text = 'Параграф';
    },

    task3: function () {
      this.text = 'Текст';
    },

    task4: function () {
      this.text = 'Заголовок';
    }
  }
}
</script>

<template>

<p class="box-red">
  <span> {{ text }} </span>Lorem ipsum dolor sit amet consectetur adipisicing elit. Amet qui ea repellendus ex, nihil quos sapiente dolores expedita assumenda ipsa blanditiis est magnam animi aut, in mollitia vitae repudiandae tempore!
  Lorem ipsum  sit amet consectetur adipisicing elit. Amet qui ea repellendus ex, nihil quos sapiente dolores expedita assumenda ipsa blanditiis est magnam animi aut, in mollitia vitae repudiandae tempore!
</p>

<p class="box-blue">
  <span> {{ text }} </span>Lorem ipsum dolor sit amet consectetur adipisicing elit. Amet qui ea repellendus ex, nihil quos sapiente dolores expedita assumenda ipsa blanditiis est magnam animi aut, in mollitia vitae repudiandae tempore!
  Lorem ipsum dolor sit amet consectetur adipisicing elit. Amet qui ea repellendus ex, nihil quos sapiente dolores expedita assumenda ipsa blanditiis est magnam animi aut, in mollitia vitae repudiandae tempore!
</p>

<button class="link" @click="task2">Изменить свойство</button>
<button class="link" @click="task3">Изменить свойство</button>
<button class="link" @click="task4">Изменить свойство</button>

</template>

<style>

body {
  margin: 60px;
  font-family: Arial, Helvetica, sans-serif;
}

.box-red {
  background-color: #fc251e;
  display: inline-block;
  padding: 10px 40px;
  border-radius: 40px;
  font-weight: bold;
  margin: 20px;
}

.box-blue {
  background-color: #1e22fc;
  display: inline-block;
  padding: 10px 40px;
  border-radius: 40px;
  font-weight: bold;
  margin: 20px;
}

span {
  color: #30c702;
  background: #000;
  font-size: 15px;
  padding: 4px 10px;
  margin-right: 3px;
  border-radius: 40px;
}


.link {
  color: #30c702;
  background: #000;
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
</style>
