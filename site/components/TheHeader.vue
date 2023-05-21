<template>
  <div class="header">
    <div class="center">
      <img class="logo" src="@/assets/logo-branca.svg" />
    </div>
    <div class="text">
      <h3>Redes sociais e design para estética</h3>
      <p>Vamos impulsionar sua clínica ou consultório para o sucesso online!</p>
    </div>
    <div class="center">
      <a
        class="btn btn-dark"
        target="_blank"
        href="https://api.whatsapp.com/send/?phone=558893839112&text=Ol%C3%A1,%20vim%20do%20seu%20site,%20e%20quero%20saber%20mais%20sobre%20o%20servi%C3%A7o%20de%20*social%20media*"
        >Agendar um contato</a
      >
    </div>
  </div>
</template>

<style lang="scss" scoped>
.logo {
  max-width: 180px;
}
.center {
  display: flex;
  justify-content: center;
  padding: 1rem;
}
.header {
  background: rgb(103, 58, 182);
  background: linear-gradient(
    45deg,
    rgba(103, 58, 182, 1) 0%,
    rgba(3, 168, 243, 1) 100%
  );

  min-height: 45vh;
  padding: 1rem;
  display: flex;
  flex-direction: column;
  justify-content: space-evenly;
  .text {
    flex: 1;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    color: white;
    text-align: center;
    h3 {
      font-size: 25px;
    }
    p {
      max-width: 40vh;
      padding-top: 30px;
    }
  }
}
</style>
