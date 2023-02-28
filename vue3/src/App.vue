<script>
import Employee from './components/Employee.vue'
export default {
  components: {
    Employee
  }, 
  data() {
	return {
		users: [
			{
				id: 1,
				name: 'name1',
				salary: 100,
				age: 30,
			},
			{
				id: 2,
				name: 'name2',
				salary: 200,
				age: 40,
			},
			{
				id: 3,
				name: 'name3',
				salary: 300,
				age: 50,
			},
		],
	}
}
}
</script>


<template>
  <Employee 
  v-for="user in users"  
  :name="user.name"
  :salary="user.salary"
  :key="user.id"
  :age="user.age"
  />
</template>


<style></style>