<script>
export default {
  name: 'App',
  data() {
    return {
      items: [1, -2, 3, -4, 5],
    }
  },
  computed: {
  },
  methods: {

  }
}
</script>

<template>

  <template v-for="elem in items">
    <nav>
      <ul v-if="elem > 0">
        <li class="box">{{ elem }}</li>
      </ul>
    </nav>
  </template>

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
</style>