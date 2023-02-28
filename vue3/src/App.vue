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
    one: function () {
      document.write('Hello 1')
    },
    two: function () {
      document.write('Hello 2')
    }
  }

}
</script>


<template>
  <Employee @show1="one" @show2="two"/>
</template>


<style></style>