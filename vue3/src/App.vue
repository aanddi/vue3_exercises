<script>
export default {
  name: 'App',
  data() {
    return {
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

  <ul>
    <li v-for="(elem1, key) in items">{{ key }}</li>
  </ul>

</template>

<style>
body {
  margin: 30px;
}

.link {
  color: #050505;
  background: #02bd02;
  font-weight: bold;
  font-size: 20px;
  padding: 10px 40px;
  border-radius: 40px;
  transition: all 0.3s ease-out;
  margin: 20px;
  display: block;
}

.link:hover {
  background-color: #b60046;
  color: #0e0101;
}

.box {
  width: 300px;
  padding: 20px 10px;
  border: 1px solid #000;
  background-color: #fff;
  margin: 10px;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: row;
}

</style>