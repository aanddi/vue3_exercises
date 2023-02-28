<script>
export default {
    props: {
      name: String,
      surn: String,
      age: Number,
      bool: Boolean
    },
    data() {
        return {
        }
    }
}
</script>

<template>
<div class="block">
  <h1>{{name}}</h1>
  <h1>{{surn}}</h1>
  <h1>{{age}}</h1>
  <h1>{{bool}}</h1>
</div>
</template>


<style>
.block {
  border: 1px solid black;
  padding: 20px;
  margin: 50px;
  width: 300px;
}
</style>