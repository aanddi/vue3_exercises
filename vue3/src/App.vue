<script>
export default {
  name: 'App',
  data() {
    return {
      base: {
        user1: '100$',
        user2: '200$',
        user3: '300$',
      }
    }
  },
  computed: {
  },
  methods: {

  }
}
</script>

<template>

<ul class="box">
  <li v-for="elem in base">{{elem}}</li>
</ul>

<br>

<ul class="box">
  <li v-for="(key, elem) in base"> {{ elem }} - {{ key }}</li>
</ul>

<br>

<ul class="box">
  <li v-for="(key, elem, index) in base"> {{ elem }} - {{ key }} - {{index + 1}}</li>
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
  flex-direction: column;
}
</style>