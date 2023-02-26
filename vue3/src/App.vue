<script>
export default {
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
  },
  methods: {
    removeUser: function (id) {
      this.users = this.users.filter((user) => {
        return user.id !== id;
      })
    }
  }
}
</script>

<template>
  <table class="tb">
    <tr v-for="user in users" :key="user.id">
      <td class="block">
        <td class="block">{{ user.name }}</td> 
        <td class="block">{{ user.salary }}</td>
        <td class="block">{{ user.age }}</td>  
        <td><button class="btn" @click="removeUser(user.id)">remove</button></td>
      </td>
    </tr>
  </table>
</template>

<style>
.tb {
  margin: 0 auto;
  border: 1px solid black;
  border-radius: 30px;
  padding: 20px;
  margin-top: 40px;
}
.block {
  border: 1px solid black;
  padding: 10px;
  margin: 10px;
  display: flex;
  border-radius: 3px;
}
.btn {
  display: block;
  padding: 10px;
  background-color: black;
  border: 1px solid black;
  color: #fff;
  transition: all 0.4s ease-out;
  margin: 10px;
}
.btn:hover {
  background-color: #fff;
  color: #fd0606;
  border: 1px solid #fd0606;
}
</style>