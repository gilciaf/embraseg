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
        "3m.jpeg",
        "airSafety.jpeg", //
        "carbografit.jpeg", //
        "danny.jpeg", //
        "debstoko.jpg",
        "ecosorb.jpg",
        "honeywell.jpeg", //
        "ledan.jpg",
        "marluvas.jpeg", //
        "mgcinto.jpeg", //
        "msa.jpeg",  //
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
        "carbografit.jpeg",
        "coopama.jpeg",
        "danny.jpeg",
        "epirock.jpeg",
        "Gkv.jpeg",
        "guaxupe.jpeg",
        "honeywell.jpeg",
        "oxiteno.jpeg", //
        "paramotos.jpeg", //
        "raízen.jpeg", //
        "saomarco.jpeg", //
        "tupi.jpeg", //
        "unif.jpeg", //
         "ipe.jpg",
         "irizar.jpg"

      ],


    }),
  }
</script>
<style lang="scss" scoped>
.principal{
  h2{
    color: crimson;
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
</style>
