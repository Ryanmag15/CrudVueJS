<template>
  <header>

    <div class="wrapper">
      <nav>
      <Navbar/>
      </nav>
    </div>
  </header>

  <RouterView />
</template>

<script setup>
import { RouterLink, RouterView } from 'vue-router'
import "bootstrap"
import Navbar from "./components/Navbar.vue"


</script>

<style>
@import "../node_modules/bootstrap/dist/css/bootstrap.min.css";
</style>
