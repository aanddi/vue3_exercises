<script>
import Employee from './components/Employee.vue'
export default {
  components: {
    Employee
  }, 
  data() {
    return {
      name: 'Andrey',
		  surn: 'Kuropatkin',
      age: 19,
      bool: true,
    }
  }
}
</script>

<template>
  <Employee :name="name" :surn="surn" :age="age" :bool="bool"/>
</template>


<style></style>