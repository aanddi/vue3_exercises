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
    one: function (num1) {
      document.write(num1)
    },
    two: function (num2) {
      document.write(num2)
    }
  }

}
</script>


<template>
  <Employee @show1="one" @show2="two"/>
</template>


<style></style>