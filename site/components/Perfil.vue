<template>
  <div class="">
    <div class="frase">
      <img src="@/assets/logo.png" alt="" />
      <h6>
        Não deixe de acreditar em si mesmo e em seu potencial, pois a confiança
        é a chave para alcançar seus objetivos.
      </h6>
    </div>
    <div class="perfil">
      <div class="top">
        <img src="@/assets/giordane.jpg" alt="" />
        <h3>Giordane Oliveira</h3>
      </div>
      <div class="text">
        <p>
          Designer gráfico com mais de 5 anos de experiência no mercado. <br />
          <br />
          Durante minha trajetória, tive a oportunidade de trabalhar com mais de
          100 clientes em diversas áreas, incluindo branding, marketing digital
          e social media. <br />
          <br />
          Atualmente, meu foco está em oferecer
          <b
            >serviços especializados em mídias para redes sociais e marketing
            orgânico</b
          >, pois acredito que esse é um campo em constante evolução e com
          grande potencial de alcance e impacto.
        </p>
      </div>
    </div>
  </div>
</template>

<style lang="scss">
.frase {
  img {
    max-width: 130px;
    padding-bottom: 20px;
  }
  position: relative;
  background: #f6f6f6;
  text-align: center;
  padding: 50px 20px;
  h6 {
    font-family: "Handlee", cursive;
    font-size: 20px;
    color: #434343;
  }
}
.perfil {
  display: flex;
  align-items: center;
  img {
    width: auto;
    height: 100px;
    border-radius: 900px;
    object-fit: cover;
  }
  position: relative;
  background: #f6f6f6;
  text-align: center;
  padding: 10px;
  padding-bottom: 60px;
  h3 {
    font-size: 20px;
    color: #434343;
  }
  .text {
    padding-left: 10px;

    p {
      text-align: justify;
    }
  }
}
</style>
