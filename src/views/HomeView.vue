<template>
  <div class="my-home">
    <v-row class="text-center mt-n12 mb-n4">
      <v-col cols="12" md="12">
        <v-img
            :src="require('../assets/banner2.jpg')"
            class="my-3"
            contain
            width="100%"
        />
      </v-col>
    </v-row>
    <sobre-nos class="mt-n4" />
    <hr>
    <hello-world />
    <footer-wj />
  </div>
</template>

<script>
  import HelloWorld from '../components/HelloWorld'
  import SobreNos from '../components/SobreNos'
  import FooterWj from '../components/FooterWj'

  export default {
    name: 'HomeView',
    components: {
      HelloWorld,
      SobreNos,
      FooterWj
    },
  }
</script>
<style scoped lang="scss">
.my-home{
  hr{
    color: #7e7e7e;
    background-color: #7e7e7e;
    opacity: 0.4;
    width: 80%;
    margin-left: 10%;
  }
}
</style>
