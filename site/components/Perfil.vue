<template>
  <div class="perfil">
    <div class="top">
      <div class="image">
        <img src="@/assets/giordane.png" alt="" />
      </div>
      <div class="title">
        <p>Quem é</p>
        <h3>Giordane Oliveira</h3>
      </div>
    </div>
    <div class="text">
      <p>
        Designer gráfico com mais de 06 anos de experiência no mercado. <br />
        <br />
        Durante minha trajetória, tive a oportunidade de trabalhar com mais de
        100 clientes em diversas áreas, incluindo branding, marketing digital e
        social media. <br />
        <br />
        Atualmente, meu foco está em oferecer
        <b
          >serviços especializados em mídias para redes sociais e marketing
          orgânico</b
        >, acredito que esse é um campo em constante evolução e com grande
        potencial de alcance e impacto.
      </p>
    </div>
  </div>
</template>

<style lang="scss">
.perfil {
  .top {
    padding-top: 20px;
    display: flex;
    justify-content: center;
    align-items: center;
    .image {
      width: 25vw;
      img {
        height: auto;
        width: 100%;
      }
    }
    .title {
      padding-left: 20px;
    }
  }
  @media only screen and (min-width: 1200px) {
    .image {
      max-width: 240px;
    }
  }
  background: #f6f6f6;
  h3 {
    font-size: 30px;
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
