<script >

</script>

<template>
  <v-header>
    <img src="../assets/icons/Boutique Oliveira.jpg" alt="">
    <v-header-a>
      <a href="#Novidades"> Novidades</a>
      <a href="#Produtos"> Produtos</a>
      <a href="#Detalhes"> Detalhes</a>
      <a href="#Rodapé"> Rodapé</a>
    </v-header-a>
    <a class="shopping" href=""><img src="../assets/icons/cart-plus.svg" alt=""></a>
  </v-header>
</template>

<style scoped>
v-header{
  display: flex;
  align-items: center;
  gap: 100px;
  justify-content: center;

}
v-header img{
  width: 110px;
  border-radius: 50%;
  margin-left: 50px;
}

v-header-a a {
  text-decoration: none;
  color:#FFE1E1 ;
  padding-left: 50px;
}

v-header-a a:hover {
    text-decoration: underline;
    /* background-color: hsla(0, 12%, 94%, 0.2); */
}

.shopping img {
  width: 15%;
  background-color: #FFE1E1;
  border-radius: 0;

}
/* .v-header a { */
  /* width: 100px; */
/* } */
</style>
