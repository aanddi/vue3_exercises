<script>
export default {
  data() {
    return {
      arr: ["Русский", "Английский", "Китайский"],
      visible1: false,
      visible2: false,
      visible3: false,
    }
  },
  methods: {
    check1() {
      this.visible1 = true;
      this.visible2 = false;
      this.visible3 = false;
    },
    check2() {
      this.visible1 = false;
      this.visible2 = true;
      this.visible3 = false;
    },
    check3() {
      this.visible1 = false;
      this.visible2 = false;
      this.visible3 = true;
    },
  }
}
</script>

<template>
  <div class="wrapper">
    <div class="block">
      <div class="item">
        <input type="radio" name="radio" @click="check1">
        <label>Русский</label>
      </div>
      <div class="item">
        <input type="radio" name="radio" @click="check2">
        <label>Английский</label>
      </div>
      <div class="item">
        <input type="radio" name="radio" @click="check3">
        <label>Китайский</label>
      </div>
      <p v-if="visible1">
        Далеко-далеко за словесными горами, в стране гласных и согласных живут рыбные тексты.
      </p>
      <p v-if="visible2">
        Far, far beyond verbal mountains, in the land of vowels and consonants, fish texts live.
      </p>
      <p v-if="visible3">
        遠在語言山脈之外，在元音和輔音的土地上，魚類文本生活著。
      </p>
    </div>
  </div>
</template>

<style>
.wrapper {
  display: flex;
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
}

p {
  margin-top: 10px;
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
</style>