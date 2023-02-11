<script>
export default {
  name: 'App',
  data() {
    return {
      hrefs: [
        { href: '1.html', text: 'text1' },
        { href: '2.html', text: 'text2' },
        { href: '3.html', text: 'text3' },
      ],

      products: [
        {
          name: 'product1',
          price: 100,
          quantity: 5
        },
        {
          name: 'product2',
          price: 200,
          quantity: 4
        },
        {
          name: 'product3',
          price: 300,
          quantity: 3
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
      <li class="menu-list" v-for="elem in hrefs">
        <a :href="elem.href" class="menu-link">{{ elem.text }}</a>
      </li>
    </ul>
  </nav>

  <table>
    <tr v-for="elem in products">
      <td>{{ elem.name }}</td>
      <td>{{ elem.price }}</td>
      <td>{{ elem.quantity }}</td>
    </tr>
  </table>

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

tr,
td,
th {
  border: 1px solid #000;
}

table {
  width: 50%;
  text-align: center;
  margin-top: 50px;
}

th {
  padding: 10px;
}

td {
  padding: 5px 7px;
}
</style>