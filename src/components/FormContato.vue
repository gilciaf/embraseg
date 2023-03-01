<template>
  <div class="main">
    <div class="form">
      <h4>Mande-nos sua mensagem pelo nosso formulário:</h4>
      <form method="POST" action="https://ciaf.com.br/gilvan@ciaf.com.br">
        <v-text-field
            label="Nome:"
            type="text"
            name="nome"
            placeholder="Seu nome"
        />

        <v-text-field
            label="Email:"
            type="text"
            name="email"
            placeholder="Seu e-mail"
        />
        <v-text-field
            label="Fone:"
            type="text"
            name="fone"
            placeholder="Seu e-mail"
        />

        <v-textarea label="Sua Mensagem:" row="6" class="message"></v-textarea>
        <v-btn class="primary" type="submit">Enviar</v-btn>
      </form>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.main {
  width: 100%;
  margin-top: -1%;
  padding: 1.4% 3.5%;
  display: flex;
  justify-content: center;
  gap: 3.5rem;
  align-items: center;
  .form {
    width: 35%;
    padding: 1.4%;
    form {
      display: flex;
      flex-direction: column;
      v-text-field {
        background-color: #cf0000;
      }
      .message {
        background-color: #e9e9e9;
        padding: 1%;
      }
      .btn {
        width: 30%;
        font-size: 1.14rem;
        font-weight: 800;
        color: white;
      }
    }
  }

}

@media screen and (max-width: 450px) {
  .main {
    margin-top:4%;
    flex-direction: column;
    .form {
      width: 100%;
      text-align: center;
      h4 {
        font-size: 1.4rem;
        color:#404040;
      }
    }

  }
}
</style>
