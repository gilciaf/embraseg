<template>
  <div class="contact">
    <contato-component />
    <form-contato />
  </div>
</template>
<script>
import ContatoComponent from "@/components/ContatoComponent.vue";
import FormContato from "@/components/FormContato.vue";
export default {
  components:{
    ContatoComponent,
    FormContato
  }
}
</script>
