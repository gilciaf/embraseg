<template>
  <div class="products mt-2">
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
            width="50%"
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
            width="50%"
            alt="logos"
        />
      </v-row>
    </v-row>
  </div>
</template>
<script>
export default {
  name: 'HelloWorld',

  data: () => ({
    impermeaveis:[
        "avental.jpeg",
        "capa.jpeg",
        "motoqueiro.jpeg",
    ],
    bloqueios :[
        "bloqueio-ajustavel.png",
        "bloqueio-valvula.png",
        "cadeado-bloqueio.png",
        "garra-bloqueio.png",
        "mini-bloqueio.png",
    ],
    capacetes :[
        "capacete1.jpeg",
        "capacete2.jpeg",
        "capacete3.jpeg",
    ],
    luvas :[
        "luva1.jpeg",
        "luva2.jpeg",
        "luva3.jpeg",
        "luva4.jpeg",
        "luva5.jpeg",
    ],
    face :[
        "solda.jpeg",
        "solda2.jpeg",
        "oculos.jpeg",
        "oculos2.jpeg",
        "oculos3.jpeg",
        "oculos4.jpeg",
    ],
      }),
}
</script>
<style scoped lang="scss">
 .products{
   margin-top: 3%;
   padding-top: 1%;
   h2{
     color: crimson;
   }
   .bloqueios {
     margin-top: -1%;
     padding: 4%;
     width: 100%;
     display: flex;
     justify-content: center;
     gap:4rem;
     img{
       max-width: 14%;
     }
   }
   .impermeaveis {
     margin-top: -2.6%;
     padding: 4%;
     width: 100%;
     display: flex;
     justify-content: center;
     gap:14rem;
     img{
       max-width: 10%;
     }
   }
   .maos {
     margin-top: -2.6%;
     padding: 4%;
     width: 100%;
     display: flex;
     justify-content: center;
     gap:7rem;
     img{
       max-width: 10%;
     }
   }
   .face {
     margin-top: -2.6%;
     padding: 4%;
     width: 100%;
     display: flex;
     justify-content: center;
     gap:4rem;
     img{
       max-width: 10%;
     }
   }
   .marcas {
     margin-top: -2.1%;
     padding: 4%;
     width: 100%;
     display: grid;
     gap:2rem;
     grid-template-columns: 1fr 1fr 1fr 1fr 1fr;
     margin-left: 3.5%;
   }
 }
 @media screen and (max-width:412px) {
   .products{
     margin-top: 3%;
     padding-top: 1%;
     h2{
       color: crimson;
     }
     .bloqueios {
       margin-top: 3%;
       gap:1rem;
       img{
         max-width: 28%;
       }
     }
     .impermeaveis {
       margin-top: 1%;
       padding: 4%;
       width: 100%;
       display: flex;
       justify-content: center;
       gap:2rem;
       img{
         max-width: 21%;
       }
     }
     .maos {
       margin-top: -0.4%;
       padding: 4%;
       width: 100%;
       display: flex;
       justify-content: center;
       gap:2rem;
       img{
         max-width: 21%;
       }
     }
     .face {
       margin-top: -2.6%;
       padding: 4%;
       width: 100%;
       display: flex;
       justify-content: center;
       gap:3rem;
       img{
         max-width: 21%;
       }
     }
     .marcas {
       padding: 4%;
       width: 100%;
       display: grid;
       gap:2rem;
       grid-template-columns: 1fr 1fr 1fr 1fr 1fr;
       margin-left: 3.5%;
     }
   }
 }
</style>
