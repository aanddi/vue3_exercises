<script>
export default {
  props: {
    id: Number,
    name: String,
    surn: String,
  },
  emits: ['remove'],
  data() {
    return {
    }
  },

}

</script>

<template>
  <div class="block">
    {{ name }}
    {{ surn }}
    <button class="btn" @click="$emit('remove', id)">remove</button>
  </div>
  
</template>


<style>
.block {
  border: 1px solid black;
  padding: 20px;
  margin: 50px;
  width: 300px;
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