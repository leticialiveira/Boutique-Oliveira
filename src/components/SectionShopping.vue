<script>
</script>

<template>
<div class="description">
    <h1>Conjunto Primavera</h1>
    <ul><li>Composição material: Fibra sintética</li> <li> Tamanhos: P, M, G</li><li>Tecido: Algodão</li><li>Estilo: Casual</li><li>Origem: CN (origem)</li><li>Estampa: Rosas Vermelhas</li>
    </ul>
    <div class="description-values">
        <button >Comprar</button>
        <span>R$130,00</span>

    </div>
</div>
<img src="../assets/image/teste.jfif" alt="">

</template>

<style scoped>
.description{
    display: flex;
    flex-direction: column;
    color: #4F2D00;
    gap: 30px;
}
.description h1{
    font-family: 'Cinzel', cursive;
    font-weight: 900;
    
}
.description ul{
    list-style: circle;
}
.description button{
    background-color: #4F2D00;
    padding: 10px;
    border-radius: 10px;
    color: #FFECD2;
}

.description .description-values{
    display: flex;
    gap: 15px;
    align-items: center;
}

.description-values span{
    color: #D40000;
    font-style: italic;
}
img {
    width: 500px;
}

</style>