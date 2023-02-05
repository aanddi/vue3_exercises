<script>
export default {
  name: 'App',
  data() {
    return {
      cosnt_tomato: 69,
      cosnt_cucumbers: 48,
      cosnt_cabbage: 45,

      amount_tomato: 3,
      amount_cucumbers: 5,
      amount_cabbage: 10,
    }

  },

  computed: {
    price_totmato: function () {
      return this.cosnt_tomato * this.amount_tomato;
    },

    price_cucumbers: function () {
      return this.cosnt_cucumbers * this.amount_cucumbers;
    },

    price_cabbage: function () {
      return this.cosnt_cabbage * this.amount_cabbage;
    },

    price_total: function () {
      return this.price_cabbage + this.price_cucumbers + this.price_totmato;
    },
  },
  methods: {
    reduce: function () {
      this.amount_tomato -= 1;
      this.amount_cucumbers -= 1;
      this.amount_cabbage -= 1;
    },

    increase: function () {
      this.amount_tomato += 1;
      this.amount_cucumbers += 1;
      this.amount_cabbage += 1;
    },
  }
}
</script>

<template>
  <table>

    <caption>
      <h1>Расчет</h1>
    </caption>

    <colgroup>
      <col span="1" style="background:Khaki">
      <col style="background-color:LightCyan">
      <col style="background-color:rgb(255, 224, 224)">
      <col style="background-color:#B5FFA0">
      <col style="background-color:#FFD7AF">
      <col style="background-color:#FFBEFD">
    </colgroup>

    <thead>

      <tr>
        <th>№ п/п</th>
        <th>Наименование товара</th>
        <th>Ед. изм.</th>
        <th>Количество</th>
        <th>Цена за ед. изм., руб.</th>
        <th>Стоимость, руб.</th>
      </tr>

    </thead>
    <tbody>

      <tr>
        <td>1.</td>
        <td>Томаты свежие</td>
        <td>кг</td>
        <td>{{ amount_tomato }}</td>
        <td>{{ cosnt_tomato }}</td>
        <td>{{ price_totmato }}</td>
      </tr>

      <tr>
        <td>2.</td>
        <td>Огурцы свежие</td>
        <td>кг</td>
        <td>{{ amount_cucumbers }}</td>
        <td>{{ cosnt_cucumbers }}</td>
        <td>{{ price_cucumbers }}</td>
      </tr>

      <tr>
        <td>3.</td>
        <td>Капуста свежая</td>
        <td>кг</td>
        <td>{{ amount_cabbage }}</td>
        <td>{{ cosnt_cabbage }}</td>
        <td>{{ price_cabbage }}</td>
      </tr>

    </tbody>


    <tfoot>

      <tr style="background-color: #B8D8E1;">
        <td colspan="5" style="text-align:right" laststr="last">ИТОГО:</td>
        <td>{{ price_total }}</td>
      </tr>

    </tfoot>

  </table>
  <button class="link" @click="increase">Добавить кол-во овощей</button>
  <button class="link" @click="reduce">Уменьшить кол-во овощей</button>

</template>

<style>
body {
  margin: 30px;
}

table,
tr,
th,
td {
  border: 1px solid #000;
  border-collapse: collapse;

}

tr,
td,
th {
  border: 1px dashed #000;
}

table {
  width: 100%;
  text-align: center;

}

th {
  padding: 10px;

}

td {
  padding: 5px 7px;

}

tr:hover td {
  background: #e8edff;
}


.link {
  color: #FFBEFD;
  background: #548cc0;
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
