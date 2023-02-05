<script>
export default {
  name: 'App',
  data() {
    return {
    }
  },

  computed: {
   
  },
  methods: {
    btn: function () {
      alert("Hello world!");
    }
  }
}
</script>

<template>
<a class="link" href="https://code.mu/ru/javascript/framework/vue/book/prime/basis/events-modifiers/" onclick="event.preventDefault()">Link</a>
<button class="link" @click.once="btn">Button</button>
</template>

<style>

body {
  margin: 30px;
}

.link {
  color: #050505;
  background: #02bd02;
  font-weight: bold;
  font-size: 20px;
  padding: 10px 40px;
  border-radius: 40px;
  transition: all 0.3s ease-out;
  margin: 20px;
}

.link:hover {
  background-color: #b60046;
  color: #0e0101;
}
</style>
