<template>
  <div class="main">
    <div class="side"></div>
    <div class="text">
      <div class="topo">
        <h2>Sobre Nós:</h2>
        <img src="../assets/embraseg.png" alt="Logo">
      </div>
      <p>
        Com experiência no mercado de EPIs desde 1999, fundamos a Embraseg no início
        de 2013 com o principal foco no atendimento das necessidades dos clientes.
        Atuamos em todo território nacional com parceira das marcas mais conceituadas do mercado mundial.
      </p>
      <p>
        Linha Completa EPIs; Produtos Industriais; Artigos de Couro; Impermeáveis;
        Uniformes Profissionais; Uniformes Eletricista NR-10; Lanternas industriais e
        áreas classificadas; Roupas Químicas; Linha de Vida e artigos para altura;
        Absorventes Industriais (Ambiental)
      </p>

    </div>
    <div class="side2"></div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.main {
  width: 100%;
  display: grid;
  grid-template-columns: 15% 70% 15%;
  h2 {
    font-family: "PT Sans", sans-serif;
    color: #cf0000;
  }
  .text {
    margin-top: 4.2%;
    margin-bottom: 3.5%;
    .topo{
      img{
        width: 28%;
      }
    }
    h3 {
      font-family: "PT Sans", sans-serif;
      color: #cf0000;
    }
    p {
      font-size: 1rem;
    }
  }
  .side {
    height: 100%;
    border-left: solid 14px #cf0000;
  }
  .side2 {
    height: 100%;
    border-right: solid 14px #cf0000;
  }
}
//@media screen and (max-width: 412px) {
//  .main {
//    grid-template-columns: 9% 82% 9%;
//  }
//}
</style>