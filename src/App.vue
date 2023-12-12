<template>
  <div id="app">
    <router-link to="/">Home</router-link>
    <router-link to="/about">About</router-link>
    <router-link to="/contact">Contact</router-link>

    <router-view></router-view>
    <About/>
    <Contact/>
    <Home/>
  </div>
</template>

<script>
import About from './components/About.vue'
import Contact from './components/Contact.vue'
import Home from './components/Home.vue'

export default {
  name: 'App',
  components: {
    About,
    Contact,
    Home
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
  margin-top: 60px;
}
</style>
