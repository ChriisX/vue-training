<template>
  <div id="app">
    <BasicComponent />
    <IterationComponent />
    <InputComponent />
    <BasicAttributesComponent />
    <StyleBindingComponent />
  </div>
</template>

<script>
import BasicComponent from './components/BasicComponent.vue';
import IterationComponent from './components/IterationComponent.vue';
import InputComponent from './components/InputComponent.vue';
import BasicAttributesComponent from './components/BasicAttributesComponent.vue';
import StyleBindingComponent from './components/StyleBindingComponent.vue';

export default {
  name: 'app',
  components: {
    BasicComponent,
    IterationComponent,
    InputComponent,
    BasicAttributesComponent,
    StyleBindingComponent
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

h1, h2 {
  text-decoration: underline;
}
</style>
