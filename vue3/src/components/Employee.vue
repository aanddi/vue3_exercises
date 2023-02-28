<script>
export default {
  props: {
    show1: Number,
    show2: Number,
  },
  data() {
    return {
    }
  },
  methods: {
    showApp1: function () {
      this.$emit('show1', 12);
    },
    showApp2: function () {
      this.$emit('show2', 11);
    }
  }
}

</script>

<template>
  <div class="blocl">
    <button class="btn" @click="showApp1">One</button>
    <button class="btn" @click="showApp2">Two</button>
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