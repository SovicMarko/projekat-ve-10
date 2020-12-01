<template>
  <div id="app">
    <app-header></app-header>
    <div id="nav">
      <h1>Ovo je neki sadrzaj</h1>
    </div>
    <router-view/>
    <footer>
      <h1>Ovo je podnozje stranice</h1>
    </footer>
  </div>
</template>

<script>
import AppHeader from "@/components/AppHeader.vue"

export default {
  components: {
    AppHeader
  }
}
</script>


<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #502c47;
}

#nav a.router-link-exact-active {
  color: #460b0b;
}
</style>
