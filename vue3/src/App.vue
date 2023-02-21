<script>
export default {
  data() {
    return {
      text: [],
      text1: '',
      text2: '',
    }
  },
  methods: {
    calc: function () {
      this.text = this.text2.split(' ');
    },
    },
  }
</script>

<template>
  <div class="wrapper">
    <div class="block">
      <textarea name="text1" id="" cols="25" rows="7" v-model="text1"></textarea>
      <p>{{ text1 }}</p>
    </div>

    <div class="block">
      <textarea name="text1" id="" cols="25" rows="7" v-model="text2"></textarea>
      <button class="btn" @click="calc">Список</button>
      <ul>
        <li v-for="(paragraph, value) in text">{{value}}) {{paragraph}}</li>
      </ul>
    </div>
  </div>
</template>

<style>
.wrapper {
  display: flex;
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
  align-items: center;
}

.block_input {
  width: 200px;
  margin: 10px 10px;
  padding: 5px;
  border: 1px solid black;
  border-radius: 10px;
}

.btn {
  background-color: #fd0606;
  padding: 10px;
  border-radius: 10px;
  border: 1px solid #fd0606;
  transition: all 0.4s ease-out;
  margin-top: 10px;
}

.btn:hover {
  background-color: #fff;
  color: #fd0606;
  border: 1px solid #fd0606;
}

textarea {
  border: 1px solid black;
  padding: 0px 10px;
}

p {
  color: #fd0606;
  padding: 5px;
}

span {
  color: #000;
  font-weight: bold;
}
</style>