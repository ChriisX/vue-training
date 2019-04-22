<template>
  <div>
    <h1>Style binding component</h1>
    <h2>Class binding</h2>
    <input v-model="active" placeholder="color">
    => <span :class="active">Lorem ipsum something...</span>
    <h2>Inline-style</h2>
    <i>Use the previous input</i><br />
    Property binding: <span v-bind:style="{ color: active }">Lorem ipsum something...</span>
  </div>
</template>

<script>
export default {
  name: "StyleBindingComponent",
  data() {
    return {
      active: "blue"
    };
  }
};
</script>

<style scoped>
    .red {
        color: red;
    }
    .green {
        color: green;
    }
    .blue {
        color: blue;
    }
</style>
