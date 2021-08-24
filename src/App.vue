<template>
  <div id="app">
    <Von />
    <List/>
    <Vmodel />
    <Vbind />
    <FetchData />
    <Filter />
  </div>
</template>

<script>
import List from './components/V-if-and-V-for'
import Von from './components/V-on'
import Vmodel from './components/V-model'
import Vbind from './components/V-bind'
import FetchData from './components/Fetch-data'
import Filter from './components/Filters'

export default {
  name: 'App',
  components: {
    List,
    Von,
    Vmodel,
    Vbind,
    FetchData,
    Filter
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
}
</style>
