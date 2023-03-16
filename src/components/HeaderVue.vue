<script >

</script>

<template>
  <div class="div-header">

    <img src="../assets/icons/Boutique Oliveira.jpg" alt="">
    <div class="div-header-a">
      <a href="#Novidades"> Novidades</a>
      <a href="#Produtos"> Produtos</a>
      <a href="#Detalhes"> Detalhes</a>
      <a href="#Detalhes"> Dicas</a>
      <a href="#Rodapé"> Rodapé</a>
    </div>
    <a class="shopping" href="#Compras"><img src="../assets/icons/cart-plus.svg" alt=""></a>
</div>
</template>

<style scoped>
.div-header{
  display: flex;
  align-items: center;
  gap: 100px;
  justify-content: space-around;
  width: 100%;
}
.div-header img{
  width: 110px;
  border-radius: 50%;
}

.div-header-a{
  gap: 50px;
  display: flex;
}
.div-header-a a {
  text-decoration: none;
  color:#FFE1E1 ;
}

.div-header-a a:hover {
    text-decoration: underline;
    /* background-color: hsla(0, 12%, 94%, 0.2); */
}

.shopping img {
  width: 50px;
  /* background-color: #FFE1E1; */
  border-radius: 0;

}
</style>
