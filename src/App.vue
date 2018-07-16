<template>
  <div id="app">
    <NavMenu msg="nav menu"/>
    <SearchForm msg="search form"/>
    <Table v-bind:tableData="listData" msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
import NavMenu from './components/NavMenu.vue'
import SearchForm from './components/SearchForm.vue'
import Table from './components/Table.vue'

export default {
  name: 'app',
  components: {
    NavMenu,
    SearchForm,
    Table
  },
   data() {
        return {
          listData: [{
            date: '2016-05-02',
            name: '王小虎',
            address: '上海市普陀区金沙江路 1518 弄'
          }, {
            date: '2016-05-04',
            name: '王小虎',
            address: '上海市普陀区金沙江路 1517 弄'
          }, {
            date: '2016-05-01',
            name: '王小虎',
            address: '上海市普陀区金沙江路 1519 弄'
          }, {
            date: '2016-05-03',
            name: '王小虎',
            address: '上海市普陀区金沙江路 1516 弄'
          }]
        }
      }
  
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
