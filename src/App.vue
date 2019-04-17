<template>
  <div id="app">
    <BasicComponent />
  </div>
</template>

<script>
import BasicComponent from './components/BasicComponent.vue'

export default {
  name: 'app',
  components: {
    BasicComponent
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
