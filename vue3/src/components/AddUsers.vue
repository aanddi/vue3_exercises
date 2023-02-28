<script>
export default {
   data() {
      return {
         newName: ' ',
         newSurn: ' ',
      }
   },
   methods: {
      save() {
         this.$emit('add', this.newName, this.newSurn)
      }
   }
}
</script>

<template>
   <div class="block">
      <input class="block_input" v-model="newName">
      <input class="block_input" v-model="newSurn">
      <button class="btn" @click="save">Save</button>
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

.block_input {
   width: 200px;
   margin: 10px 10px;
   padding: 5px;
   border: 1px solid black;
   border-radius: 10px;
   display: block;
}
</style>