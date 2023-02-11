<script>
export default {
  name: 'App',
  data() {
    return {
      menu: {
        Главная: '#',
        Продукция: '#',
        Контакты: '#',
        Галлерея: '#',
      },
      items: [1, 2, 3, 4, 5],
    }
  },
  computed: {
  },
  methods: {

  }
}
</script>

<template>

  <nav>
    <ul class="menu_item">
      <li class="menu-list" v-for="(elem, key) in menu">
        <a :href="elem" class="menu-link active">{{ key }}</a>
      </li>
    </ul>
  </nav>

  <div class="wrapper">
    <div v-for="elem in items">
      <div class="box">
        <h1>{{ elem }}</h1>
        <p>
          Далеко-далеко за словесными горами в стране гласных и согласных живут рыбные тексты. Деревни которой
          реторический
          злых ipsum, дорогу то. Прямо, несколько знаках грустный переулка то маленький жаренные страну дороге решила
          правилами вдали?
        </p>
      </div>
    </div>
  </div>

  <div class="wrapper">
    <div v-for="elem in items">
      <div class="box">
        <h1>{{ elem }}</h1>
        <p>
          Далеко-далеко за словесными горами в стране гласных и согласных живут рыбные тексты. Деревни которой
          реторический
          злых ipsum, дорогу то. Прямо, несколько знаках грустный переулка то маленький жаренные страну дороге решила
          правилами вдали?
        </p>
      </div>
    </div>
  </div>

</template>

<style>
nav {
  margin-top: 20px;
}

.menu_item {
  display: flex;
  justify-content: center;
}

.menu-list {
  list-style: none;
  margin-right: 10px;
  font-weight: bold;
}

.menu-link {
  text-decoration: none;
  color: #ffffff;
  background-color: #16A177;
  border: 1px solid #16A177;
  padding: 10px 25px;
  transition: all 0.4s ease-out;
  border-radius: 10px;
}

.menu-link:hover {
  background-color: #fff;
  border: 1px solid #16A177;
  color: #16A177;
}

.box {
  width: 300px;
  padding: 20px 20px;
  border: 1px solid #000;
  background-color: #fff;
  margin: 10px;
  display: flex;
  align-items: center;
  flex-direction: column;
  text-align: justify;
  transition: all 0.4s ease-out;

}

.wrapper {
  display: flex;
  flex-direction: row;
  justify-content: center;
  margin-top: 50px;
}

.box:hover {
  background-color: #16A177;
  color: #fff;
  border: 1px solid #fff;
}
</style>