<script>
export default {
  name: 'App',
  data() {
    return {
      user: 'Andrey Kuropatkin'
    }
  },
  methods: {
    show: function () {
      alert(this.user);
    }
  }
}
</script>

<template>

 {{ show() }}

</template>

<style>
body {
  margin: 60px;
  font-family: Arial, Helvetica, sans-serif;
}

.box {
  background-color: #fc251e;
  display: inline-block;
  padding: 10px 40px;
  border-radius: 40px;
  font-weight: bold;
}


.link {
  background: red;
  font-weight: bold;
  font-size: 20px;
  padding: 20px 30px;
  border-radius: 40px;
  transition: all 0.3s ease-out;
}

.link:hover {
  background-color: #000;
  color: red;
}
</style>
