<script>
export default {
    props: ['arg'],
    data() {
        return {
        }
    }
}
</script>

<template>
<ul class="block">
    <li v-for="item in arg">{{ item }}</li>
</ul>
</template>


<style>
.block {
  border: 1px solid black;
  padding: 20px;
  margin: 50px;
  width: 300px;
}
</style>