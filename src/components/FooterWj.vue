vue
<template>
  <div class="main">
    <div class="linha"></div>
    <div class="extrutura">
      <div class="address">
        <div class="logo">
          <img src="../assets/logo-cinza.png" width="100%" alt="Logo WS" />
        </div>
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
    <div class="developer" style="color: #d9d8d8">
      <h6>Desenvolvimento:</h6>
      <h5>Ciaf Soluções em Software</h5>
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
    gap: 7rem;
    justify-content: center;
    align-items: center;
    margin-top: 4%;

    .address {
      color: white;
      margin-left: 3%;
      .logo {
        //background-color: white;
        padding: 1%;
        width: 77%;
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
      margin-right: 3%;
    }
    .vertical-line {
      min-height: 100%;
      min-width: 0.14%;
      background-color: white;
      color: white;
    }
  }
  .developer {
    margin-top: 2%;
  }
}
@media screen and (max-width:450px) {
  .main {
    .extrutura {
      flex-direction: column;
      gap: 1rem;
      .address {
        color: white;
        margin-left: 7%;
        .logo {
          padding: 2%;
          width: 28%;
        }
      }
      .social-medias {
        width: 95%;
        background-color: #9f0404;
        padding: 2.1% 2.8% 0 2.1%;
        display: flex;
        justify-content: space-around;
        margin-left: 4%;
        h3{
          font-size: 1rem;
        }
        img{
          width: 90%;
          margin-right: 2.1%;
        }
      }
    }
  }
}
</style>
