<script setup>
import { RouterLink, RouterView } from "vue-router";
import Header from "./components/Header.vue";
</script>

<template>
  <div>
    <Header msg="Pokedex" />
  </div>
</template>

<style>
@import "@/assets/base.css";
@import "@/assets/normalize.css";

#app {
  background: #262835;
  font-weight: normal;
  margin: 0 auto;
  padding: 2rem;
}
</style>
