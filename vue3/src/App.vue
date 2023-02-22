<script>
export default {
  data() {
    return {
      isDisabled: true,
      isDisabled1: true,
      checked: false,
    }
  },
  methods: {
    toggle: function () {
      this.isDisabled = false;
    },
    toggle1: function () {
      this.isDisabled1 = false;
    },
  }
}
</script>

<template>
  <div class="wrapper">
    <input type="text" class="block_input" placeholder="andrey" v-bind:disabled="isDisabled">
    <button class="btn" @click="toggle">btn</button>

    <input type="text" class="block_input" placeholder="kuropatkin" v-bind:disabled="isDisabled1">
    <input type="checkbox" class="block_input " v-model="checked" @click="toggle1">
    <button class="btn" @click="toggle">btn</button> 
  </div>
</template>

<style>
.wrapper {
  
}

label {
  margin-left: 6px;
}

.block {
  border: 1px solid black;
  padding: 30px 30px;
  width: 300px;
  margin: 20px 30px;
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
  background-color: #fd0606;
  padding: 10px;
  border-radius: 10px;
  border: 1px solid #fd0606;
  transition: all 0.4s ease-out;
  margin-top: 10px;
  display: block;
}

.btn:hover {
  background-color: #fff;
  color: #fd0606;
  border: 1px solid #fd0606;
}
</style>