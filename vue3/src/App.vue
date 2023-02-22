<script>
export default {
  data() {
    return {
      newItem: '',
      items: ['a', 'b', 'c', 'd', 'e'],
    }
  },
  methods: {
    addFirstItem: function () {
     this.items.unshift(this.newItem);
    },
    addlastItem: function () {
     this.items.push(this.newItem);
    }
  }
}
</script>

<template>
  <ul>
    <li v-for="(item, index) in items" :key="index">
      {{ item }}
    </li>
  </ul>
  <input v-model="newItem" class="block_input">
  <button @click="addFirstItem" class="btn">add first</button>
  <button @click="addlastItem" class="btn">add last</button>
</template>

<style>
.block {
  border: 1px solid black;
  padding: 30px 30px;
  width: 300px;
  margin: 20px 10px;
  text-align: justify;
  display: flex;
  justify-content: center;
  flex-direction: column;
}

.block_input {
  width: 200px;
  margin: 10px 10px;
  padding: 5px;
  border: 1px solid black;
  border-radius: 10px;
  display: block;
}

.btn {
  display: block;
  width: 200px;
  text-align: center;
  background-color: #fd0606;
  padding: 10px 40px;
  border-radius: 20px;
  border: 1px solid #fd0606;
  transition: all 0.4s ease-out;
  margin: 20px 10px;
}

.btn:hover {
  background-color: #fff;
  color: #fd0606;
  border: 1px solid #fd0606;
}

ul {
  margin-left: 20px;
}
</style>