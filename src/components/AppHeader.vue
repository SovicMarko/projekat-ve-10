<template>
  <nav class="navbar navbar-inverse">
    <div class="container-fluid">
        <div class="navbar-header">
            <router-link to="/" class="navbar-brand">Moja Aplikacija</router-link>
        </div>
        <ul class="nav navbar-nav">
            <li><router-link to="/">Home</router-link></li>
            <li><router-link to="/about">O nama</router-link></li>
            <li><router-link to="/contact">Kontakt</router-link></li>
        </ul>
        <ul class="nav navbar-nav navbar-right">
            <li><a href="#"><span class="glyphicon glyphicon-user"></span> Sign Up</a></li>
            <li><a href="#"><span class="glyphicon glyphicon-log-in"></span> Login</a></li>
        </ul>
    </div>
    </nav>
</template>

<script>
export default {
    name: "AppHeader"
}
</script>

<style scoped>
    .navbar {
        border-radius: 0px;
    }
</style>