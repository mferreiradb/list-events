<script setup>
import { RouterLink, RouterView } from 'vue-router'

</script>

<template>
  <header>
    <div id="layout">
      <div class="wrapper">
        <nav>
          <RouterLink to="/">Home</RouterLink> | 
          <RouterLink to="/about">About</RouterLink>
        </nav>
      </div>
      <RouterView />
    </div>
  </header>
</template>

<style>
#layout {
  font-family: Acvenir, Helvetica, sans-serif;
  -webkit-font-smoothing: antialiased;
  -webkit-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #2c3e50
}

nav a.router-link-exact-active {
  color: #42b983;
}
h2 {
  font-size: 20px;
}
</style>
