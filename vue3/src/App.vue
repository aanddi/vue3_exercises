<script>
export default {
  data() {
    return {
      selected: '',
    }
  },
  methods: {

  }
}
</script>

<template>
  <div class="wrapper">
    <div class="block">
      <select v-model="selected">
        <option>value1</option>
        <option>value2</option>
        <option>value3</option>
      </select>

      <p>{{ selected }}</p>
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

select {
  border: 1px solid black;
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