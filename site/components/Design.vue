<template>
  <div id="design" class="">
    <div class="header">
      <p>Conheça meu trabalho de</p>
      <h1>Social Media</h1>
    </div>
    <div class="carrossel">
      <img src="@/assets/posts/post1.jpg" alt="" />
      <img src="@/assets/posts/post2.jpg" alt="" />
      <img src="@/assets/posts/post3.jpg" alt="" />
      <img src="@/assets/posts/post4.jpg" alt="" />
      <img src="@/assets/posts/post5.jpg" alt="" />
      <img src="@/assets/posts/post6.jpg" alt="" />
      <img src="@/assets/posts/post7.jpg" alt="" />
      <img src="@/assets/posts/post8.jpg" alt="" />
      <img src="@/assets/posts/post9.jpg" alt="" />
      <img src="@/assets/posts/post10.jpg" alt="" />
    </div>

    <div class="topicos">
      <div class="topico">
        <h4>Elaboração do contéudo</h4>
        <p>
          Elaboramos conteúdos relevantes para o seu negócio que ajudarão
          aumentar o engajamento e alcance da sua marca nas redes sociais.
          <br /><br />
          Com base nas necessidades e interesses do seu público-alvo, eu vou
          criar <b> conteúdo que seja relevante e de valor</b> para eles.
          <br /><br />
          Além disso, vou medir os resultados da sua estratégia de conteúdo para
          ajustá-la sempre que necessário.
        </p>
      </div>
      <div class="topico">
        <h4>Cronograma de postagens</h4>
        <p>
          <b>
            Segunda, quarta e sexta.
            <br />
            Terças e quintas.
            <br />
            Te quinta a domingo.
          </b>

          <br /><br />
          Seu négocio é dinâmico e seu cronograma de postagens também precisa
          ser !
          <br /><br />
          Escolha a quantidade de posts para cada mês e vamos juntos planejar as
          estratégias para montar um cronograma e aproveitar as melhores datas
          para promover além de conteúdo,
          <b
            >promoções, datas comemorativas eventos que façam sentido no seu
            negócio.</b
          >
          <br /><br />Você escolhe o que postar e quando!
        </p>
      </div>
      <div class="topico">
        <h4>Agendamento de Posts</h4>
        <p>
          <i
            >Postar todo dia no mesmo horário é difícil, mas ter consistencia é
            importante! </i
          ><br />
          <br />
          organizar fotos, legendas, hastags, <b>deixe essa parte comigo</b> e
          tenha mais tranquilidade na gestão do seu negócio.
          <br />
          <br />Basta aprovar o cronograma de postagens que os posts serão
          programados no seu instagram e facebook.
        </p>
      </div>

      <div class="topico">
        <h4>Stories</h4>
        <p>
          <i
            >Os stories são a forma de engajar mais organicamente com seus
            seguidores, o conteúdo dos stories deve complementar o feed. </i
          ><br />
          <br />
          Por isso os planos <b>First Impression</b> e
          <b>Brand Booster</b> oferecem versões de story de
          <b> 05 e 10</b> posts respectivamente, e você pode escolher quantos
          quiser no plano <b>Made on demand</b>.
          <br />
          <br /><b>O que são as versões de story?</b> <br />
          As versão de story vão complementar seu post do feed com o foco em
          engajamento.
          <br />
          Vamos fazer <b>enquentes, abrir caixas de perguntas</b>, e entregar
          algo a mais sobre o conteudo do feed, de uma forma rapida e dinâmica.
        </p>
      </div>
    </div>
    <div class="header">
      <p>Confira alguns</p>
      <h1>Clientes</h1>
    </div>
    <div class="clientes">
      <a href="https://www.instagram.com/patriciafroesmeyer/">
        <img src="@/assets/clientes/irg.jpg" alt="" />
      </a>
      <a href="https://www.instagram.com/dra.marcelajorge/">
        <img src="@/assets/clientes/marcela.jpg" alt="" />
      </a>
      <a href="https://www.instagram.com/vivianicarrer/">
        <img src="@/assets/clientes/viviani.jpg" alt="" />
      </a>
      <a href="https://www.instagram.com/clinicaeternapro/">
        <img src="@/assets/clientes/eterna.jpg" alt="" />
      </a>
      <a href="https://www.instagram.com/lcandrada/">
        <img src="@/assets/clientes/luis.jpg" alt="" />
      </a>
      <a href="https://www.instagram.com/centrokappa/">
        <img src="@/assets/clientes/kappa.jpg" alt="" />
      </a>
    </div>
  </div>
</template>

<style lang="scss">
#design {
  .header {
    padding: 2rem;
    h1 {
      font-size: 45px;
    }
  }
  .carrossel {
    display: flex;
    overflow-x: auto;
    overflow-y: hidden;
    white-space: nowrap;

    img {
      height: 200px;
      padding: 5px;
      padding-bottom: 20px;
      background: white;
      margin-left: 10px;
    }
  }
  color: white;
  background: #3571d4;
  .clientes {
    padding: 2rem;
    display: grid;
    display: grid;
    grid-template-columns: 1fr 1fr;
    grid-template-rows: 1fr;
    gap: 10px 10px;
    grid-template-areas: ". .";
    justify-content: center;
    align-content: center;
    justify-items: center;
    align-items: center;
    justify-self: center;
    img {
      width: 100%;
      height: auto;
      border-radius: 10px;
    }
  }
  .topicos {
    padding: 1rem;
    .topico {
      h4 {
        font-size: 22px;
        padding-bottom: 20px;
      }
      padding: 1rem;
      margin-bottom: 2rem;
      border-radius: 1rem;
      background: rgb(103, 58, 182);
      background: linear-gradient(45deg, #4782e1 0%, #3571d4 60%);
    }
  }
}
</style>
