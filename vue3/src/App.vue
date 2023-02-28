<script>
import Employee from './components/Employee.vue'
export default {
  components: {
    Employee
  }, 
  data() {
	return {

   } },
  methods: {
    one: function (name) {
      document.write(name)
    },
    two: function (name, salary) {
      document.write(name + '  ' + salary)
    }
  }

}
</script>


<template>
  <Employee @show1="one" @show2="two"/>
</template>


<style></style>