<template>
  <div class="main">
    <div class="wj">
      <v-card elevation="7" class="card-contato">
        <h3 class="text-md-center">Fale Direto:</h3>
        <div class="contato mt-4">
          <img src="../assets/socialmedia/whatsapp-3.svg" width="20px" alt="whatsapp" />
          <h4 class="mt-2">(35) 99135-0066</h4>
        </div>
        <div class="contato mt-2">
          <img src="../assets/socialmedia/email-3.svg" width="20px" alt="whatsapp" />
          <h4 class="mt-2">walter@embraseg.net</h4>
        </div>
      </v-card>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.main {
  margin-top: 1%;
  padding: 1.4%;
  display: flex;
  flex-direction: column;
  align-items: center;
  .wj {
    width: 28%;
    .card-contato {
      padding: 2.8% 0%;
      .contato {
        width: 100%;
        display: flex;
        align-items: center;
        justify-content: center;
        gap: 0.5rem;
        img {
          width: 10%;
        }
      }
    }
  }
}
@media screen and (max-width: 450px) {
  .main {
    margin-top: 1%;
    .wj{
      width: 100%;
      .card-contato{
        h3{
          margin-left: 4%;
        }
      }
    }
  }
}
</style>
