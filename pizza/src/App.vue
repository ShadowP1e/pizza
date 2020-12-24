<template>
<div id="app">
<app-pizza v-bind:pizzaName='pizzaName' v-bind:pizzaPrice='pizzaPrice' v-bind:pizzaSize='pizzaSize'>
<div slot='content'>
<ul>
  <li>Бекон</li>
  <li>Свежие томаты</li>
  <li>Соус</li>
  <li>Сыр Моцарелла</li>
  <li>Сыр Пармезан</li>
</ul>
</div>
</app-pizza>
</div>
</template>
<script>
import Pizza from './components/Pizza.vue'

export default {
  name: 'app',
  data(){
    return {
      pizzaName: 'ШПицца от Школы программистов',
      pizzaPrice: 600,
      pizzaSize: '28cm',
    }
  },
  components: {
    appPizza: Pizza
  } 
}
</script>
<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
  display: flex;
  border: 1px solid black;
  width: 400px;
}
li{
  padding: 5px;
}
</style>
