<template>
  <div class="card-carrinho">
    <h1>{{ msg }}</h1>

    <div class="lista-itens">
      <div class="item">
        <a href="https://github.com/vuejs/vue-cli/tree/dev/packages/%40vue/cli-plugin-eslint" target="_blank" rel="noopener">
          <img alt="Vue logo" src="../assets/logo.png">
        </a>
        <div class="produto">
          <h4>Nome do BomBOM</h4>
          <div>R$: 00,00</div>

        </div>
      </div>
      <div class="item">
        <a href="https://github.com/vuejs/vue-cli/tree/dev/packages/%40vue/cli-plugin-eslint" target="_blank" rel="noopener">
          <img alt="Vue logo" src="../assets/logo.png">
        </a>
        <div class="produto">
          <h4>Nome do BomBOM</h4>
          <div>R$: 00,00</div>

        </div>
      </div>
    </div>
    <div class="total">
      <div  class="nome-total">
      <h4> Total</h4>
      </div>
      <div class="nome-total" >
       <h4> R$: 00,00</h4>
      </div>

    </div>
    <div class="promocao">
      <span>Parabéns, sua compra tem frete grátis !</span>
    </div>
    <div class="btn">
      <button class="btn-finalizar-compra">Finlizar Compra</button>
    </div>

  </div>


</template>

<script>
  export default {
    name: 'HelloWorld',
    props: {
      msg: String
    }
  }
</script>


<style scoped>

  .card-carrinho{
    background-color: #FFFFFF;
    margin-left: auto;
    margin-right: auto;
    border-radius: 5px;
    width: 600px;
    border: 1px solid #2c3e50;

  }
  .card-carrinho > h1{
    margin-top: 0.25rem;
    padding: 10px;
    border-bottom: 1px solid #2c3e50;
  }

  .card-carrinho > .lista-itens > a{
    display: flex;
    text-align: start;
  }
  .card-carrinho > .lista-itens > a > img{
    width:100%;
    height: auto;
  }
  .lista-itens{
    flex-direction: row;
    /*display: flex;*/
    flex-wrap: wrap;
    border-bottom: 1px solid #2c3e50;

  }
  .item{
    flex: 1;
    flex-direction: row;
    text-align: start;
    border-bottom: 1px solid #2c3e50;
    display: flex;
  }
  .produto{
    position: relative;
  }
  .total{
    padding: 5px;
    display: flex;
    justify-content: space-between;
    flex-direction: row;

  }
  .nome-total{
    font-weight: 600;
    flex: 0 0 25%;
  }
  .promocao{
    font-weight: bolder;
    margin: 20px;
    flex: 1;

  }
  .promocao> span{
    border-radius: 10px;
    background-color: #49ff71;
    color: #0b5119;
    padding: 10px;

  }
  .btn{
    margin: 15px;
  }
  .btn-finalizar-compra{
    margin-top: 20px;
    width: 100%;
    border-color: #4675ff;
    border-radius: 5px;
    color: #FFF;
    background-color: #4675ff;
    padding: 5px;
    font-size: 1.3rem;
    font-weight: bold;

  }

  h3 {
    margin: 20px 0 0;
  }
  ul {
    list-style-type: none;
    padding: 0;
  }
  li {
    display: inline-block;
    margin: 0 10px;
  }
  a {
    color: #42b983;
  }
</style>
