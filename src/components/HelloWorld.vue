<template>
  <div class="principal">
    <h2 class="text-center">Nossos parceiros:</h2>
    <v-row class="marcas">
      <img
          v-for="(logo, index) in paths" :key="index"
          :src="require('../assets/logos/' + logo)"
          width="50%"
          alt="logos"
      />
    </v-row>
    <h2 class="text-center">Alguns de Nossos Clientes:</h2>
    <v-row class="marcas">
      <img
          v-for="(logo, index) in clients" :key="index"
          :src="require('../assets/logos/' + logo)"
          width="50%"
          alt="logos"
      />
    </v-row>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',

  data: () => ({
    paths: [
      "danny.jpeg", //
      "msa.jpeg",  //
      "3m.jpeg",
      "airSafety.jpeg", //
      "carbografit.jpeg", //
      "debstoko.jpg",
      "ecosorb.jpg",
      "honeywell.jpeg", //
      "ledan.jpg",
      "marluvas.jpeg", //
      "mgcinto.jpeg", //
      "nutriex.jpeg", //
      "sayro.jpeg", //
      "streammylight.jpeg", //
      "ultrasafe.jpeg", //
      "vicsa.jpeg", //
      "wwuniformes.jpeg", //
    ],
    clients: [
      "alcoa.jpeg",
      "angloAmerican.jpeg",
      "coopama.jpeg",
      "epirock.jpeg",
      "Gkv.jpeg",
      "guaxupe.jpeg",
      "oxiteno.jpeg", //
      "paramotos.jpeg", //
      "raízen.jpeg", //
      "saomarco.jpeg", //
      "tupi.jpeg", //
      "unif.jpeg", //
      "ipe.jpg",
      "irizar.jpg",
      "destak.jpeg",
      "frivasa.jpeg",
      "unifenas.jpeg"

    ],


  }),
}
</script>
<style lang="scss" scoped>
.principal{
  h2{
    color: #9b0927;
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
@media screen and (max-width: 450px) {
  .principal{
    h2{
      color: #9b0927;
    }
    .marcas {
      margin-top: -2.1%;
      padding: 4%;
      width: 100%;
      display: grid;
      gap:2rem;
      grid-template-columns: 1fr 1fr 1fr 1fr 1fr;
      margin-left: 3.5%;
      img{
        width: 90%;
      }
    }
  }
}
</style>
