<template>
  <div>
    <h1>Basic attributes component</h1>
    <h2>v-once</h2>
    <button @click="increment">Increment value</button>
    <ul>
      <li>With v-once: <span v-once>{{ value }}</span></li>
      <li>Without v-once: <span>{{ value }}</span></li>
    </ul>
    <h2>v-html</h2>
    <ul>
      <li>With v-html: <span v-html="rawHTML"></span></li>
      <li>Without v-html: <span>{{ rawHTML }}</span></li>
    </ul>
    <h2>v-bind</h2>
    <button :disabled="disabled">Disabled button</button>
    <h2>v-if / ternary</h2>
    <button @click="toggle">Toggle {{ display ? 'off' : 'on'}}</button><br />
    <span v-if="display">I'm a light and I'm on</span>
  </div>
</template>

<script>
export default {
  name: "BasicAttributesComponent",
  data() {
    return {
      value: 0,
      rawHTML: "<strong>text</strong>",
      disabled: true,
      display: true
    }
  },
  methods: {
    increment: function() {
      this.value++;
    },
    toggle: function() {
      this.display = !this.display;
    }
  }
};
</script>

<style scoped>
ul {
  list-style-type: none;
  padding: 0;
}

span {
  display: inline-block;
  margin: 5px;
}
</style>
