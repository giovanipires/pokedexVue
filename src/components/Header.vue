<script setup>
defineProps({
  msg: {
    type: String,
    required: true,
  },
});
</script>

<template>
  <div>
    <div class="header">
      <img alt="pokedex image" class="logo" src="@/assets/pokedex.png" />
      <h1 class="white">{{ msg }}</h1>
      <input class="search" type="text" placeholder="  Buscar Pokemon..." />
    </div>
  </div>
</template>

<style scoped>
@import "@/assets/normalize.css";
.header {
  align-items: center;
  display: flex;
  justify-content: center;
  height: 300px;
}
.logo {
  height: 47px;
  position: absolute;
  margin-top: 40px;
  margin-left: -231px;
  width: 47px;
}
.white {
  color: rgb(247, 247, 247);
  font-size: 40px;
  font-style: italic;
  font-weight: 900;
  line-height: 37.5px;
  position: relative;
  margin-top: 65px;
  margin-left: 15px;
  text-decoration: none;
  transition: 0.4s;
}
.search {
  background: rgba(255, 255, 255, 0.2);
  border-radius: 10px;
  border-style: none;
  height: 50px;
  margin-top: 167px;
  position: fixed;
  width: 600px;
}
</style>
