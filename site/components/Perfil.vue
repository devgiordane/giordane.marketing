<template>
  <div class="perfil">
    <div class="left"></div>
    <div class="text">
      <p>Quem é</p>
      <h3>Giordane Oliveira</h3>
      <p>
        Designer gráfico com mais de 5 anos de experiência no mercado. <br />
        <br />
        Durante minha trajetória, tive a oportunidade de trabalhar com mais de
        100 clientes em diversas áreas, incluindo branding, marketing digital e
        social media. <br />
        <br />
        Atualmente, meu foco está em oferecer
        <b
          >serviços especializados em mídias para redes sociais e marketing
          orgânico</b
        >, pois acredito que esse é um campo em constante evolução e com grande
        potencial de alcance e impacto.
      </p>
    </div>
  </div>
</template>

<style lang="scss">
.perfil {
  display: flex;
  align-items: stretch;
  .left {
    min-width: 25vw;
    background-size: cover;
    background-position: bottom;
    background-image: url("@/assets/giordane.jpg");
  }
  background: #f6f6f6;
  h3 {
    font-size: 20px;
    color: #434343;
  }
  .text {
    padding: 3rem 1rem;
    h3 {
      font-size: 30px;
      padding-bottom: 30px;
    }
    p {
      text-align: justify;
    }
  }
}
</style>
