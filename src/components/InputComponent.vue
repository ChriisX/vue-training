<template>
    <div>
        <h1>Input component</h1>
        <input type="text" v-model="name" placeholder="Your name...">
        <p>Your name is <span>{{ name }}</span></p>
    </div>
</template>

<script>
export default {
    name: "InputComponent",
    data() {
        return {
            name: "Christophe"
        }
    }
}
</script>

<style scoped>
    span {
        font-weight: bold;
    }
</style>
