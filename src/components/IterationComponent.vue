<template>
  <div>
    <h1>Iteration component</h1>
    <button v-on:click="addRandomItem">Add random item</button>
    <ul>
      <li v-for="item in items" :key="item.id">{{ item.text }}</li>
    </ul>
  </div>
</template>

<script>
import uuid from "uuid";

export default {
  name: "IterationComponent",
  data() {
    return {
      items: [
        {
          id: 1,
          text: "First Item"
        },
        {
          id: 2,
          text: "Second Item"
        }
      ]
    };
  },
  methods: {
    addRandomItem() {
      const value = uuid();
      this.items.push({ id: value, text: value });
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
