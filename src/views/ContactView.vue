<template>
  <div class="contact">
    <contato-component />
    <form-contato />
    <footer-wj />
  </div>
</template>
<script>
import ContatoComponent from "@/components/ContatoComponent.vue";
import FormContato from "@/components/FormContato.vue";
import FooterWj from '../components/FooterWj'
export default {
  components:{
    ContatoComponent,
    FormContato,
    FooterWj
  }
}
</script>
