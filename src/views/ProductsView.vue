<template>
  <div class="products mt-2">
    <v-row class="text-center mt-n16 mb-n4">
      <v-col cols="12" md="12">
        <v-img
            :src="require('../assets/banner3.jpg')"
            class="my-3"
            contain
            width="100%"
        />
      </v-col>
    </v-row>
    <h2 class="text-center mt-2">Linha de Produtos:</h2>
    <v-row justify="center">
      <h3 class="mt-4">Bloqueios:</h3>
      <v-row class="bloqueios">
        <img
            v-for="(produto, index) in bloqueios" :key="index"
            :src="require('../assets/produtos/' + produto)"
            width="50%"
            alt="logos"
        />
      </v-row>
    </v-row>
    <v-row justify="center">
      <h3 class="mt-1">Impermeáveis:</h3>
      <v-row class="impermeaveis">
        <img
            v-for="(produto, index) in impermeaveis" :key="index"
            :src="require('../assets/produtos/impermeaveis/' + produto)"
            width="77%"
            height="auto"
            alt="logos"
        />
      </v-row>
    </v-row>
    <v-row justify="center">
      <h3 class="mt-1">Proteção de Cabeça:</h3>
      <v-row class="impermeaveis">
        <img
            v-for="(produto, index) in capacetes" :key="index"
            :src="require('../assets/produtos/capacetes/' + produto)"
            width="50%"
            alt="logos"
        />
      </v-row>
    </v-row>
    <v-row justify="center">
      <h3 class="mt-1">Proteção de Mãos:</h3>
      <v-row class="maos">
        <img
            v-for="(produto, index) in luvas" :key="index"
            :src="require('../assets/produtos/luvas/' + produto)"
            width="50%"
            alt="logos"
        />
      </v-row>
    </v-row>
    <v-row justify="center">
      <h3 class="mt-1">Proteção de Face:</h3>
      <v-row class="face">
        <img
            v-for="(produto, index) in face" :key="index"
            :src="require('../assets/produtos/face/' + produto)"
            alt="logos"
            width="50%"
        />
      </v-row>
    </v-row>
    <v-row justify="center">
      <h3 class="mt-n1">Calçados Segurança:</h3>
      <v-row class="botas">
        <img
            v-for="(produto, index) in botas" :key="index"
            :src="require('../assets/produtos/botas/' + produto)"
            width="50%"
            alt="logos"
        />
      </v-row>
    </v-row>
    <v-row justify="center">
      <h3 class="mt-1">Roupas NR-10:</h3>
      <v-row class="nr10">
        <img
            v-for="(produto, index) in nr10" :key="index"
            :src="require('../assets/produtos/nr10/' + produto)"
            width="50%"
            alt="logos"
        />
      </v-row>
    </v-row>
    <v-row justify="center">
      <h3 class="lant-pc mt-1">Lanternas Área Controlada(Intrissicamente Segura):</h3>
      <h3 class="lant-mobile mt-1">Lanternas Área Controlada:</h3>
      <v-row class="lanternas">
        <img
            v-for="(produto, index) in lanternas" :key="index"
            :src="require('../assets/produtos/lanternas/' + produto)"
            width="70%"
            height="70%"
            alt="logos"
        />
      </v-row>
    </v-row>
    <v-row justify="center" class="mt-n7">
      <h3 class="mt-n1">Proteção a Quedas:</h3>
      <v-row class="quedas">
        <img
            v-for="(produto, index) in contraQuedas" :key="index"
            :src="require('../assets/produtos/contra-quedas/' + produto)"
            width="50%"
            alt="logos"
        />
      </v-row>
    </v-row>
    <v-row justify="center">
      <h3 class="mt-1">Proteção Respiratória:</h3>
      <v-row class="botas">
        <img
            v-for="(produto, index) in respiratorio" :key="index"
            :src="require('../assets/produtos/respiratorio/' + produto)"
            width="50%"
            alt="logos"
        />
      </v-row>
    </v-row>
    <v-row justify="center">
      <h3 class="mt-1">Proteção Auricular:</h3>
      <v-row class="botas">
        <img
            v-for="(produto, index) in auricular" :key="index"
            :src="require('../assets/produtos/auricular/' + produto)"
            width="50%"
            alt="logos"
        />
      </v-row>
    </v-row>
    <footer-wj class="mt-4" />
  </div>
</template>
<script>
import FooterWj from '../components/FooterWj'
export default {
  name: 'HelloWorld',
  components:{
    FooterWj
  },

  data: () => ({
    impermeaveis: [
      "capa.jpeg",
      "avental3.jpeg",
      "motoqueiro.jpeg",
    ],
    bloqueios: [
      "bloqueio-ajustavel.png",
      "bloqueio-valvula.png",
      "cadeado-bloqueio.png",
      "garra-bloqueio.png",
      "mini-bloqueio.png",
    ],
    capacetes: [
      "capacete1.jpeg",
      "capacete2.jpeg",
      "capacete3.jpeg",
    ],
    luvas: [
      "luva1.jpeg",
      "luva2.jpeg",
      "luva3.jpeg",
      "luva4.jpeg",
      "luva5.jpeg",
    ],
    face: [
      "solda.jpeg",
      "solda2.jpeg",
      "oculos.jpeg",
      "oculos2.jpeg",
      "oculos3.jpeg",
      "oculos4.jpeg",
    ],
    botas: [
      "bota1.jpeg",
      "bota2.jpeg",
      "bota3.jpeg",
      "bota4.jpeg",
      "bota5.jpeg",
    ],
    nr10: [
      "conjunto1.jpeg",
      "conjunto2.jpeg",
    ],
    lanternas: [
      "lanterna4.jpeg",
      "lanterna2.jpeg",
      "lanterna3.jpeg",
    ],
    contraQuedas: [
      "contraqueda1.jpeg",
      "contraqueda2.jpeg",
      "contraqueda3.jpeg",
      "contraqueda4.jpeg",
      "contraqueda5.jpeg",
    ],
    respiratorio: [
      "respiratorio.jpeg",
      "respiratorio2.jpeg",
      "respiratorio3.jpeg",
      "respiratorio4.jpeg",
      "respiratorio5.jpeg",
    ],
    auricular: [
      "auricular1.jpeg",
      "auricular2.jpeg",
      "auricular3.jpeg",
      "auricular4.jpeg",
      "auricular5.jpeg",
    ],
  }),
}
</script>
<style scoped lang="scss">
.products {
  margin-top: 3%;
  padding-top: 1%;

  h2 {
    color: crimson;
  }

  .bloqueios {
    margin-top: -1%;
    padding: 4%;
    width: 100%;
    display: flex;
    justify-content: center;
    gap: 4rem;

    img {
      max-width: 14%;
    }
  }

  .impermeaveis {
    margin-top: -2.6%;
    padding: 4%;
    width: 120%;
    height: 120%;
    display: flex;
    justify-content: center;
    gap: 14rem;

    img {
      max-width: 12%;
      max-height: 80%;
    }
  }

  .maos {
    margin-top: -2.6%;
    padding: 4%;
    width: 100%;
    display: flex;
    justify-content: center;
    gap: 7rem;

    img {
      max-width: 10%;
    }
  }

  .face {
    margin-top: -2.6%;
    padding: 4%;
    width: 100%;
    height: 100%;
    display: flex;
    justify-content: center;
    gap: 2.1rem;
    img {
      max-width: 14%;
      height: 50%;
    }
  }

  .botas {
    margin-top: -2.6%;
    padding: 4%;
    width: 100%;
    display: flex;
    justify-content: center;
    gap: 7rem;

    img {
      max-width: 10%;
    }
  }
  .quedas {
    margin-top: -2.6%;
    padding: 4%;
    width: 100%;
    display: flex;
    justify-content: center;
    gap: 7rem;

    img {
      max-width: 10%;
    }
  }
  .lant-mobile{
    display: none;
  }
  .lanternas {
    margin-top: -2.6%;
    padding: 4%;
    width: 100%;
    display: flex;
    justify-content: space-around;
    gap: 4rem;

    img {
      max-width: 8%;
    }
  }
  .nr10 {
    margin-top: -2.6%;
    padding: 4%;
    width: 100%;
    display: flex;
    justify-content: center;
    gap: 4rem;
    img {
      max-width: 18%;
    }
  }

  .marcas {
    margin-top: -2.1%;
    padding: 4%;
    width: 100%;
    display: grid;
    gap: 2rem;
    grid-template-columns: 1fr 1fr 1fr 1fr 1fr;
    margin-left: 3.5%;
  }
}

@media screen and (max-width: 450px) {
  .products {
    margin-top: 3%;
    padding-top: 1%;

    h2 {
      color: crimson;
    }

    .bloqueios {
      margin-top: 3%;
      gap: 1rem;

      img {
        max-width: 28%;
      }
    }

    .impermeaveis {
      margin-top: 1%;
      padding: 4%;
      width: 100%;
      display: flex;
      justify-content: center;
      gap: 2rem;

      img {
        max-width: 21%;
      }
    }

    .maos {
      margin-top: -0.4%;
      padding: 4%;
      width: 100%;
      display: flex;
      justify-content: center;
      gap: 2rem;

      img {
        max-width: 21%;
      }
    }

    .face {
      margin-top: -2.6%;
      padding: 4%;
      width: 100%;
      display: flex;
      justify-content: center;
      gap: 3rem;

      img {
        max-width: 21%;
      }
    }

    .botas {
      margin-top: -1.2%;
      padding: 4%;
      width: 100%;
      display: flex;
      justify-content: center;
      gap: 4rem;

      img {
        max-width: 18%;
      }
    }
    .quedas {
      margin-top: -1.2%;
      padding: 4%;
      width: 100%;
      display: flex;
      justify-content: center;
      gap: 4rem;

      img {
        max-width: 18%;
      }
    }
    .lant-mobile{
      display: block;
    }
    .lant-pc{
      display: none;
    }
    .lanternas {
      margin-top: -2.6%;
      padding: 4%;
      width: 100%;
      display: flex;
      justify-content: center;
      gap: 4rem;

      img {
        max-width: 14%;
        height: 35%;
      }
    }

    .nr10 {
      margin-top: -2.6%;
      padding: 4%;
      width: 100%;
      display: flex;
      justify-content: center;
      gap: 4rem;

      img {
        max-width: 28%;
      }
    }

    .marcas {
      padding: 4%;
      width: 100%;
      display: grid;
      gap: 2rem;
      grid-template-columns: 1fr 1fr 1fr 1fr 1fr;
      margin-left: 3.5%;
    }
  }
}
</style>
