<template>

  <carrinho-compras msg="Meu carrinho"/>
</template>

<script>
import CarrinhoCompras from './components/CarrinhoCompras.vue'

export default {
  name: 'App',
  components: {
    CarrinhoCompras
  }
}
</script>

<style>
  @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@100&display=swap');
html{
  background-color: #27aed8;
}
#app {
  font-family: 'Poppins', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
