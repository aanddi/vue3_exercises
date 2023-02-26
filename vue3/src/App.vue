<script>
export default {
  data() {
    return {
      arr: ['a', 'b', 'c', 'd']
    }
  },
  methods: {
    removeItem: function (index)  {
      this.arr.splice(index, 1)
    }
  }
}
</script>

<template>
  <ul>
    <li class="block" @click="removeItem(index)" v-for="(item, index) in arr" :key="index">
      {{ item }}
    </li>
  </ul>

 
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

.block:hover{
  background-color: #000;
  color: #fff;
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