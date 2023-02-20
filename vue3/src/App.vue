<script>
export default {
  data() {
    return {
      message: 'hello',
      number: 2,
      obj: {
        block: true,
        uppercase: true
      },
    }
  },
  methods: {

  }
}
</script>

<template>
	<input v-model="message" class="block_input">
	<p :class="obj">{{ message }}</p>

  <input v-model="number" class="block_input">
	<p :class="obj">{{ number**2 }}</p>


</template>

<style>
.block {
  border: 1px solid black;
  padding: 20px;
  width: 300px;
  margin: 20px 30px;
  text-align: justify;
}

.block_input {
  width: 300px;
  margin: 20px 30px;
  padding: 10px;
  border: 1px solid black;
  border-radius: 10px;
}

.color.bg {
  color: green;
  background-color: yellow;
}

.bold.cursive {
  font-weight: bold;
  font-style: italic;

}

.uppercase {
  text-transform: uppercase;
}

</style>