<script>
export default {
  data() {
    return {
      check: true,

    }
  }
}
</script>

<template>
  <div class="wrapper">
    <div class="block">
      <input type="checkbox" v-model="check">
      <p v-if="check">Андрей Куропаткин</p>
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


</style>