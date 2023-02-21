<script>
export default {
  data() {
    return {
      check: [],

    }
  }
}
</script>

<template>
  <div class="wrapper">
    <div class="block">
      <div class="item">
        <input type="checkbox" v-model="check" name="1" value="Русский">
        <label for="1">Русский</label>
      </div>
      <div class="item">
        <input type="checkbox" v-model="check" name="2" value="Английский">
        <label for="2">Английский</label>
      </div>
      <div class="item">
        <input type="checkbox" v-model="check" name="3" value="Китайский">
        <label for="3">Китайский</label>
      </div>
      <div class="item">
        <input type="checkbox" v-model="check" name="4" value="Татарский">
        <label for="4">Татарский</label>
      </div>
    <ul>
      <li v-for="(l, v) in check">{{v}}) {{l}}</li>
    </ul>
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

ul {
  margin-top: 10px;
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


</style>