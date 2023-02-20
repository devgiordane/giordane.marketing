<template>
  <div class="footer">
    <div class="center">
      <img class="logo" src="@/assets/logo-branca.svg" />
    </div>
    <div class="center">
      <a
        class="btn btn-white"
        target="_blank"
        href="https://api.whatsapp.com/send/?phone=558893839112&text=Ol%C3%A1,%20vim%20do%20seu%20site,%20e%20quero%20saber%20mais%20sobre%20o%20servi%C3%A7o%20de%20*social%20media*"
        >Agendar um contato</a
      >
    </div>
    <div class="social">
      <a href="https://www.instagram.com/giordane_oliveira">
        <img src="@/assets/instagram.png" alt="" />
      </a>
      <a
        href="https://api.whatsapp.com/send/?phone=558893839112&text=Ol%C3%A1,%20vim%20do%20seu%20site,%20e%20quero%20saber%20mais%20sobre%20o%20servi%C3%A7o%20de%20*social%20media*"
      >
        <img src="@/assets/whatsapp.png" alt="" />
      </a>
      <a href="https://www.youtube.com/@giordanemarketing"></a>
      <img src="@/assets/youtube.png" alt="" />
    </div>
    <div class="text">
      <p class="small">
        Giordane Oliveira - 2023. <br />
        Todos os direitos reservados.
      </p>
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
.footer {
  background: rgb(103, 58, 182);
  background: linear-gradient(
    45deg,
    rgba(103, 58, 182, 1) 0%,
    rgba(3, 168, 243, 1) 100%
  );
  padding: 1rem;
  .social {
    display: flex;
    padding: 2rem 5rem;
    justify-content: space-evenly;
    img {
      height: 20px;
    }
  }
  .text {
    .small {
      font-size: 11px;
    }
    flex: 1;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    color: white;
    text-align: center;
  }
}
</style>
