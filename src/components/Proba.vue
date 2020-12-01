<template>
    <div>
      <h1>Ovo je proba</h1>
      <h2>{{broj}}</h2>
      <button v-on:click="broj++">+</button>
    </div>
</template>

<script>
export default {
    name: "proba",
    data: function() {
        return {
            broj : 5
        }
    }
}
</script>

<style scoped>
    h1 {
        color: blueviolet;
    }
</style>