<template>
  <div>
    <h1>Basic component</h1>
    <span v-bind:title="title">{{ message }}</span>
    <span v-if="visible">This message is visible</span>
  </div>
</template>

<script>
export default {
  name: "BasicComponent",
  data() {
    return {
      message: "Hello Vue!",
      title: "You loaded this page on " + new Date().toLocaleString(),
      visible: true
    };
  }
};
</script>

<style>
span {
  display: block;
}
</style>
