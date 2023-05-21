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
      <img src="@/assets/posts/post11.jpg" alt="" />
      <img src="@/assets/posts/post12.jpg" alt="" />
    </div>

    <div class="topicos">
      <div class="topico">
        <h4>Elaboração do contéudo</h4>
        <p>
          Conteúdos relevantes para o seu negócio que ajudarão a aumentar o
          engajamento e o alcance da sua marca nas redes sociais. <br />
          Com base nas necessidades e interesses do seu público-alvo, eu vou
          criar um conteúdo que seja valioso e relevante para eles. <br /><br />
          Vamos medir os resultados da sua estratégia de conteúdo para ajustá-la
          sempre que necessário
        </p>
      </div>
      <div class="topico">
        <h4>Cronograma de postagens</h4>
        <p>
          <b>
            Segundas, quartas e sextas; terças e quintas; de quinta a
            domingo.</b
          >
          <br />
          <br />
          Seu negócio é dinâmico e seu cronograma de postagens também precisa
          ser! Com o nosso serviço, você pode escolher a quantidade de posts que
          deseja por mês e juntos planejaremos estratégias para montar um
          cronograma que aproveite as melhores datas para promover não apenas
          conteúdo, mas também promoções, eventos e datas comemorativas que
          façam sentido para o seu negócio. <br />
          Você escolhe o que postar e quando!
        </p>
      </div>
      <div class="topico">
        <h4>Agendamento de Posts</h4>
        <p>
          <i
            >Postar todo dia no mesmo horário pode ser difícil, mas ter
            consistência é fundamental para o sucesso nas redes sociais! </i
          ><br />
          <br />
          Deixe a organização de fotos, legendas e hashtags comigo e tenha mais
          tranquilidade na gestão do seu negócio. <br />
          Basta aprovar o cronograma de postagens e os posts serão programados
          no seu Instagram e Facebook.
        </p>
      </div>

      <div class="topico">
        <h4>Reels</h4>
        <p>
          <i>Tenha mais alcance e gere autoridade com seu conteúdo</i>
          <br />
          <br />
          <b>
            Os vídeos curtos são a principal fonte de conteúdo que as pessoas
            buscam nas redes sociais, e ficar fora dessa tendência é limitar seu
            potêncial
          </b>
          <br />
          <br />
          O planos First Impression e Brand Booster oferecem
          <b>04 reels</b>, e no plano Made on Demand você pode escolher quantos
          quiser. <br /><br />
        </p>
      </div>
      <div class="topico">
        <h4>Stories</h4>
        <p>
          <i
            >Os stories são uma forma orgânica de engajar com seus seguidores, e
            o conteúdo dos stories deve complementar o que é postado no feed.</i
          >
          <br />
          <br />
          Por isso, os nossos planos First Impression e Brand Booster oferecem
          <b>07 storys</b>, e no plano Made on Demand você pode escolher quantos
          quiser. <br /><br />
          <b> Mas o que são essas versões de stories? </b>
          <br />
          <br />
          Elas complementam o post do feed com o foco em engajamento. <br />
          Vamos fazer enquetes, caixas de perguntas e entregar algo a mais sobre
          o conteúdo do feed, de forma rápida e dinâmica.
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
  background: #2f2f2f;
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
      background: linear-gradient(17deg, #444444 0%, #2f2f2f 40%);
    }
  }
  @media only screen and (min-width: 1200px) {
    .carrossel {
      img {
        height: 400px;
      }
    }
    .clientes {
      padding: 3rem;
      grid-template-columns: 1fr 1fr 1fr;
      grid-template-rows: 1fr;
      gap: 10px 10px;
      grid-template-areas: ". . .";
    }
  }
}
</style>
