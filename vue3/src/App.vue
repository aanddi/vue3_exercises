<script>
export default {
  name: 'App',
  data() {
    return {
      text: 'page',
      href: 'page.html',
    }
  }
}
</script>

<template>

<a :href="href" class="link"> {{ text }} </a>

</template>

<style>

body {
  margin: 60px;
  font-family: Arial, Helvetica, sans-serif;
}

.link {
  background: red;
  font-weight: bold;
  font-size: 20px;
  padding: 20px 50px;
  border-radius: 40px;
  transition: all 0.3s ease-out;
}

.link:hover {
  background-color: #000;
  color: red;
}

</style>
