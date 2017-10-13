<template>
  <div class="container" id="app">
      <FactorySelection v-on:factoryChanged="factoryChanged"></FactorySelection>
      <DateSelection></DateSelection>
      <ShiftSelection></ShiftSelection>
  </div>
</template>

<script>
import FactorySelection from './components/FactorySelection'
import DateSelection from './components/DateSelection'
import ShiftSelection from './components/ShiftSelection'

export default {
  name: 'app',
  components: {
    FactorySelection,
    DateSelection,
    ShiftSelection
  },
  data () {
    return {
      factory: ""
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
