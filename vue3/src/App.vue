<script>
export default {
  data() {
    return {
      text1: "text",
      text2: "text2",
      none: false,
    }
  },
  methods: {
    submit: function () {
      this.text1 = this.$refs.textField.value;
    },
    ctrl: function (event) {
      if (event.ctrlKey) {
        this.none = true;
      }
    },
    right: function (event) {
      if (!event.ctrlKey) {
        this.text2 = 'right';
      }
    },
    left: function (event) {
      if (!event.ctrlKey) {
        this.text2 = 'left';
      }
    },
    middle: function (event) {
      if (!event.ctrlKey) {
        this.text2 = 'middle';
      }
    },
  }
}
</script>

<template>
  <input type="text" @keyup.enter="submit" class="block_input" ref="textField" />
  <p class="block">{{ text1 }}</p>

  <br>

  <a href="#" class="btn" @click="ctrl">link</a>
  <p class="block" v-if="none">{{ text2 }}</p>

  <br>

  <a href="#" class="btn" @click.right="right" @click.left="left" @click.middle="middle">link</a>
  <p class="block">{{ text2 }}</p>
</template>

<style>
.wrapper {}

label {
  margin-left: 6px;
}

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
  margin: 20px 20px;
}

.btn:hover {
  background-color: #fff;
  color: #fd0606;
  border: 1px solid #fd0606;
}
</style>