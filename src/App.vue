<script setup>
import { RouterLink, RouterView } from 'vue-router'
import myFooter from './components/myFooter.vue'
</script>

<template>
  <header>
    <nav class="navbar navbar-expand-sm">      
        <div class="container-fluid">
          <h3 class="ml-5 font-weight-bold">Portfolio</h3>

          <div class="drop">
            <img src="./assets/icon-menu.svg" class="mr-5">
            <div class="menu">
              <RouterLink to="/" id="link">Home</RouterLink>
              <RouterLink to="/about" id="link">About</RouterLink>
              <RouterLink to="/skills" id="link">Skills</RouterLink>
              <RouterLink to="/projects" id="link">Projects</RouterLink>
            </div>
          </div>
        </div>
    </nav>  
  </header>

  <RouterView />

  <footer>
    <myFooter />
  </footer>
</template>

<style scoped>
  header {
    background-color: darkcyan;
  }
  img {
    height: 20px;
    width: 30px;
  }

  .menu {
    z-index: 1;
    position: absolute;
    right: 30px;
    padding: 0;
    display: none;
    width: 100px;
    background-color: white; 
  }

  .menu #link {
    display: block;
    padding: 10px;
    text-decoration: none;
    color: black;
  }

  .drop:hover .menu {
    display: block;
  }
</style>
