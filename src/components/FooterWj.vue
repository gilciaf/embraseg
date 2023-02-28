vue
<template>
  <div class="main">
    <div class="linha"></div>
    <div class="extrutura">
      <div class="address">
        <div class="logo">
          <img src="../assets/embraseg.png" width="88%" alt="Logo WS" />
        </div>
        <h3 style="color: white">WJ Representações</h3>
        <h4>Avenida Juscelino Kubitschek, 220</h4>
        <h4>Bairro Parque Vivaldi Leite Ribeiro</h4>
        <h4>Cep: 37701-186- Poços de Caldas MG</h4>
      </div>
      <div class="vertical-line"></div>
      <div class="social-medias">
        <h3>Conheça nossa página no Facebook</h3>
        <a href="https://web.facebook.com/embraseg.net?_rdc=1&_rdr">
          <img
              src="../assets/facebook.svg"
              width="70px"
              class="ml-2"
              alt="Facebook"
          />
        </a>

      </div>
    </div>
    <div class="linha" style="margin-top: 4%"></div>
    <div class="developer" style="color: #b6b6b6">
      <h6>Ciaf Soluções em Software</h6>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.main {
  background-color: #9f0404;
  padding: 2.8% 1.4% 1% 1.4%;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  .linha {
    height: 1px;
    width: 100%;
    background-color: white;
  }
  .extrutura {
    display: flex;
    gap: 1rem;
    justify-content: space-around;
    align-items: center;
    margin-top: 4%;

    .address {
      color: white;
      margin-left: 7%;
      .logo {
        background-color: white;
        padding: 2%;
        width: 14%;
        display: flex;
        justify-content: center;
        align-items: center;
        border-radius: 10px;
      }
    }
    .social-medias {
      width: 100%;
      color: white;
      background-color: #ab0108;
      padding: 3.5% 1.4% 1% 1.4%;
      display: flex;
      justify-content: center;
      align-items: center;
      gap: 0.7rem;
      margin-right: 7%;
    }

    .vertical-line {
      min-height: 100%;
      min-width: 0.14%;
      background-color: white;
      color: white;
    }
  }
  .developer {
    margin-top: 4%;
  }
}
@media screen and (max-width:412px) {
  .main {
    .extrutura {
      flex-direction: column;
      gap: 1rem;
      .address {
        color: white;
        margin-left: 7%;
        .logo {
          background-color: white;
          padding: 2%;
          width: 28%;
        }
      }
      .social-medias {
        width: 100%;
        background-color: #9f0404;
        padding: 1.4% 1.4% 1% 1.4%;
        display: flex;
        justify-content: center;
        gap: 1rem;
        margin-left: 7%;
        img{
          width: 80%;
        }
      }
    }
  }
}
</style>
