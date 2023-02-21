<script>
export default {
  data() {
    return {
      options: ['Понедельник', 'Вторник', 'Среда', 'Четверг', 'Пятница', 'Суббота', 'Воскресенье'],
      selected: '',
      selected1: '',
      selected2: '',
      selected3: '',
      selected4: '',
      selected5: '',
      selected6: '',
      
      day: '',
      month: '',
      year: '',

      options1: ['1', '2', '3', '4', '5', '6', '7', '8', '9', '10', '11', '12',
       '13', '14', '15', '16', '17', '18', '19', '20', '21', '22', '23', '24',
        '25', '26', '27', '28', '29', '30', ' 31'],
      options2: ['Январь', 'Февраль','Март', 'Апрель', 'Май','Июнь', 'Июль', 'Август', 'Сентябрь', 'Октябрь', 'Ноябрь', 'Декабрь'],
      options3: ['2023', '2022','2021', '2020', '2019','2018']
    }
  },
  methods: {
    today: function () {
      const date = new Date();
      this.day = String(date.getDate());
      this.month = String(date.getMonth() + 1);
      this.year = date.getFullYear();
    }
    
  }
}
</script>

<template>
  <div class="wrapper">
    <div class="block">
      <select v-model="selected">
        <option v-for="i in options">{{ i }}</option>
      </select>
      <p>{{ selected }}</p>
    </div>

    <div class="block">
      <select v-model="selected1">
        <option v-for="i in options1">{{ i }}</option>
      </select>
      <select v-model="selected2">
        <option v-for="i in options2">{{ i }}</option>
      </select>
      <select v-model="selected3">
        <option v-for="i in options3">{{ i }}</option>
      </select>
      <p>{{ selected1 + ' ' + selected2 + ' ' + selected3 }}</p>
    </div>

    <div class="block">
      <select v-model="selected4">
        <option>{{day}}</option>
      </select>
      <select v-model="selected5">
        <option>{{month}}</option>
      </select>
      <select v-model="selected6">
        <option>{{year}}</option>
      </select>
      <button @click="today" class="btn">Today</button>
      <p>{{ selected4 + '.' + selected5 + '.' + selected6 }}</p>
  </div>
  </div>
</template>

<style>
.wrapper {
  display: flex;
}

label {
  margin-left: 6px;
}

.block {
  border: 1px solid black;
  padding: 30px 30px;
  width: 300px;
  margin: 20px 30px;
  text-align: justify;
  display: flex;
  justify-content: center;
  flex-direction: column;
}

.block_input {
  width: 200px;
  margin: 10px 10px;
  padding: 5px;
  border: 1px solid black;
  border-radius: 10px;
}

select {
  border: 1px solid black;
  margin-top: 10px;
}

p {
  margin-top: 10px;
}

.btn {
  background-color: #fd0606;
  padding: 10px;
  border-radius: 10px;
  border: 1px solid #fd0606;
  transition: all 0.4s ease-out;
  margin-top: 10px;
}

.btn:hover {
  background-color: #fff;
  color: #fd0606;
  border: 1px solid #fd0606;
}
</style>