<script setup>
defineProps({
  msg: {
    type: String,
    required: true
  }
});
</script>

<template>
  <div>
    <div class="header">
      <div class="logo">
        <img alt="pokedex image" src="@/assets/pokedex.png" />
        <h1>{{ msg }}</h1>
      </div>
      <input type="search" placeholder="Buscar Pokemon..." />
    </div>
  </div>
</template>

<style scoped lang="scss">
@import "@/assets/normalize.css";
.header {
  display: flex;
  align-items: center;
  justify-content: center;
  flex-flow: column;
}
.logo {
  display: flex;
  align-items: center;
  justify-content: center;
  flex-wrap: wrap;
  margin: 30px;

  img {
    width:100px;
    margin-left: 30px;
    margin-right: 30px;
  }

  h1 {
    color: rgb(247, 247, 247);
    font-size: 40px;
    margin: unset;
    font-style: italic;
    font-weight: 900;
    transition: 0.4s;
  }
}


  /* o input agora é type="search", que é um tipo de input que pode servir pra barras de busca! */
  /* -------- https://www.w3schools.com/tags/att_input_type_search.asp -------- */

  /* com esse "seletor de atributos" você não precisa da classe .search para selecionar o input */
  /* -- https://developer.mozilla.org/pt-BR/docs/Web/CSS/Attribute_selectors -- */

input[type="search"]  {
  background: rgba(255, 255, 255, 0.2);
  border-radius: 10px;
  border-style: none;
  padding: 1rem;
  width: 100%;
  max-width: 600px;
}

</style>
