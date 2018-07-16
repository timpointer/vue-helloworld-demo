<template>
  <div id="app">
    <NavMenu msg="nav menu"/>
    <SearchForm msg="search form"/>
    <Table msg="Welcome to Your Vue.js App"/>
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
