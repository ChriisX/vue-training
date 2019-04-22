<template>
  <div>
    <h1>Basic attributes component</h1>
    <h2>v-once</h2>
    <button @click="increment">Increment value</button>
    <ul>
      <li>With v-once: <span v-once>{{ value }}</span></li>
      <li>Without v-once: <span>{{ value }}</span></li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "BasicAttributesComponent",
  data() {
    return {
      value: 0
    }
  },
  methods: {
    increment: function() {
      this.value++;
    }
  }
};
</script>

<style scoped>
ul {
  list-style-type: none;
  padding: 0;
}
</style>
