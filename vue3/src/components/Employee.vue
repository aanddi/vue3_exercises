<script>
export default {
  props: {
    id: Number,
    name: String,
    surn: String,
  },
  emits: ['change'],
  data() {
    return {
      isEdit: false,
      newName: this.name,
      newSurn: this.surn,
    }
  },
  methods: {
    edit() {
      this.isEdit = true;
    },
    save() {
      this.isEdit = false;
      this.$emit('change', this.id, this.newName, this.newSurn);
    }
  }
}
</script>

<template>
  <template v-if="!isEdit">
    <div class="block">
      <h1>{{ name }}</h1>
      <h1>{{ surn }}</h1>
      <button class="btn" @click="edit">edit</button>
    </div>
  </template>
  <template v-else>
    <div class="block">
      <input class="block_input" v-model="newName">
      <input class="block_input" v-model="newSurn">
      <button class="btn" @click="save">save</button>
    </div>
  </template>
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

.block_input {
  width: 200px;
  margin: 10px 10px;
  padding: 5px;
  border: 1px solid black;
  border-radius: 10px;
  display: block;
}
</style>