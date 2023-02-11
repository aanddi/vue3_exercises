<script>
export default {
  name: 'App',
  data() {
    return {
      products: [
        {
          id: 2,
          name: 'product1',
        },

        {
          id: 3,
          name: 'product2',
        },

        {
          id: 1,
          name: 'product3',
        },
      ]
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
      <li class="menu-list" v-for="elem in products" :key="products.id">
        <a href="#" class="menu-link active">{{ elem.name }}</a>
      </li>
    </ul>
  </nav>

</template>

<style>
nav {
  margin-top: 40px;
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
</style>