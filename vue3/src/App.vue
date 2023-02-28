<script>
import Employee from './components/Employee.vue'
export default {
  components: {
    Employee
  }
}
</script>

<template>
  <Employee :arg="{ a: 1, b: 2, c: 3 }" />
</template>


<style></style>