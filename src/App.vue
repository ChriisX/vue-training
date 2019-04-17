<template>
  <div id="app">
    <BasicComponent />
    <IterationComponent />
  </div>
</template>

<script>
import BasicComponent from './components/BasicComponent.vue';
import IterationComponent from './components/IterationComponent.vue';

export default {
  name: 'app',
  components: {
    BasicComponent,
    IterationComponent
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
