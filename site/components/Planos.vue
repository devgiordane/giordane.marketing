<template>
  <div class="planos">
    <h2 class="plan-title">Escolha um dos planos de social media</h2>
    <div class="plano">
      <h2 class="bg2">First Impression</h2>
      <h3><span>R$</span>270<span>/mês</span></h3>
      <p class="subtitle">
        A primeira impressão é a que fica, e eu quero te ajudar a ter um perfil
        rico em conteúdo de qualidade para apresentar ao público os valores,
        diferenciais e vantagens da sua marca, produto ou serviço.
      </p>
      <div class="body">
        <div class="features">
          <div class="feature"><p>Fotos para Feed</p></div>
          <div class="feature"><p>Reels</p></div>
          <div class="feature"><p>Versão Story</p></div>
          <div class="feature"><p>Agendamento de Posts</p></div>
          <div class="feature"><p>Elaboração do contéudo</p></div>
          <div class="feature"><p>Suporte</p></div>
        </div>
        <div class="values">
          <div class="value"><p>12 por mês</p></div>
          <div class="value"><p>04 por mês</p></div>
          <div class="value"><p>04 por mês</p></div>
          <div class="value"><p>Sim</p></div>
          <div class="value"><p>Sim</p></div>
          <div class="value">
            <p>Das 8h às 18h, Seg. a Sáb., via WhatsApp</p>
          </div>
        </div>
      </div>
      <div class="btnspace">
        <a
          target="_blank"
          href="https://api.whatsapp.com/send/?phone=558893839112&text=Ol%C3%A1,%20vim%20do%20seu%20site,%20e%20quero%20saber%20mais%20sobre%20o%20plano%20*First%20Impression*!"
          class="btn btn-dark"
          >Quero saber mais</a
        >
      </div>
    </div>
    <div class="plano bg1">
      <h2 class="">Brand Booster</h2>
      <h3><span>R$</span>377<span>/mês</span></h3>
      <p class="subtitle">
        Ideal para você que está querendo consilidar sua marcar e gerar
        autoridade, com 25 posts por mês vamos ter uma grande frequência de
        conteudo no seu feed, para fixar bem sua marca para seu seguidores.
      </p>
      <div class="body">
        <div class="features">
          <div class="feature"><p>Posts no Feed</p></div>
          <div class="feature"><p>Reels</p></div>
          <div class="feature"><p>Versão Story</p></div>

          <div class="feature"><p>Agendamento de Posts</p></div>
          <div class="feature"><p>Elaboração do contéudo</p></div>
          <div class="feature"><p>Suporte</p></div>
        </div>
        <div class="values">
          <div class="value"><p>20 por mês</p></div>
          <div class="value"><p>04 por mês</p></div>
          <div class="value"><p>05 por mês</p></div>
          <div class="value"><p>Sim</p></div>
          <div class="value"><p>Sim</p></div>
          <div class="value">
            <p>Das 8h às 18h, Seg. a Sáb., via WhatsApp</p>
          </div>
        </div>
      </div>
      <div class="btnspace">
        <a
          target="_blank"
          href="https://api.whatsapp.com/send/?phone=558893839112&text=Ol%C3%A1,%20vim%20do%20seu%20site,%20e%20quero%20saber%20mais%20sobre%20o%20plano%20*Brand%20Booster*!"
          class="btn btn-light"
          >Quero saber mais</a
        >
      </div>
    </div>
    <div class="plano bg2">
      <h2 class="">Made on demand</h2>
      <h3><span>R$</span>{{ customPreco }}<span>/mês</span></h3>
      <p class="subtitle">
        Costumize seu plano conforme a necessidade, toda a liberdade que você
        precisa para escolher melhor atende sua necessidades.
      </p>
      <div class="body">
        <div class="features">
          <div class="feature"><p>Posts no Feed</p></div>
          <div class="feature"><p>Reels</p></div>
          <div class="feature"><p>Versão Story</p></div>

          <div class="feature"><p>Agendamento de Posts</p></div>
          <div class="feature"><p>Elaboração do contéudo</p></div>
          <div class="feature"><p>Suporte</p></div>
        </div>
        <div class="values">
          <div class="value">
            <button
              @click="qtd.posts > 0 ? qtd.posts-- : qtd.posts"
              class="btn-increase"
            >
              -</button
            ><span class="field">{{ qtd.posts }}</span
            ><button @click="qtd.posts++" class="btn-increase">+</button>
          </div>

          <div class="value">
            <button
              @click="qtd.reels > 0 ? qtd.reels-- : qtd.reels"
              class="btn-increase"
            >
              -</button
            ><span class="field">{{ qtd.reels }}</span
            ><button @click="qtd.reels++" class="btn-increase">+</button>
          </div>
          <div class="value">
            <button
              @click="qtd.stories > 0 ? qtd.stories-- : qtd.stories"
              class="btn-increase"
            >
              -</button
            ><span class="field">{{ qtd.stories }}</span
            ><button @click="qtd.stories++" class="btn-increase">+</button>
          </div>
          <div class="value">
            <input
              type="checkbox"
              v-model="qtd.agendamento"
              id="agendamento"
            /><label for="agendamento">agendamento</label>
          </div>
          <div class="value">
            <input type="checkbox" v-model="qtd.conteudo" id="conteudo" /><label
              for="conteudo"
              >conteudo</label
            >
          </div>

          <div class="value">
            <p>Das 8h às 18h, Seg. a Sáb., via WhatsApp</p>
          </div>
        </div>
      </div>
      <div class="btnspace">
        <a
          target="_blank"
          :href="`https://api.whatsapp.com/send/?phone=558893839112&text=Ol%C3%A1,%20vim%20do%20seu%20site,%20e%20quero%20saber%20mais%20sobre%20o%20plano%20*Made%20on%20demand*!\n\n\ ${msg}`"
          class="btn btn-light"
          >Quero saber mais</a
        >
      </div>
    </div>
  </div>
</template>

<script lang="ts">
export default {
  data: function () {
    return {
      qtd: {
        posts: 12,
        stories: 4,
        reels: 4,
        agendamento: true,
        conteudo: true,
      },
    };
  },
  computed: {
    customPreco: function () {
      let preco = 0;
      let qtd = this.qtd;
      if (qtd.posts) {
        preco += qtd.posts * 10;
      }

      if (qtd.stories) {
        preco += qtd.stories * 3;
      }
      if (qtd.reels) {
        preco += qtd.reels * 15;
      }

      if (qtd.agendamento) {
        preco += 30;
      }

      if (qtd.conteudo) {
        preco += (qtd.posts + qtd.reels) * 3;
      }
      return preco;
    },
    msg: function () {
      let m = "";
      let qtd = this.qtd;
      if (qtd.posts > 0) {
        m += `\n\n ✅ Com ${qtd.posts}  posts`;
      }

      if (qtd.stories > 0) {
        m += `\n\n ✅ Com ${qtd.stories}  stories`;
      }
      if (qtd.reels > 0) {
        m += `\n\n ✅ Com ${qtd.reels}  Reels`;
      }

      if (qtd.agendamento) {
        m += `\n\n ✅ Agendamento de posts`;
      }

      if (qtd.conteudo) {
        m += `\n\n ✅ Elaboração de conteúdo!`;
      }
      return encodeURI(m);
    },
  },
};
</script>

<style lang="scss">
.planos {
  background: white;
  .plan-title {
    font-size: 25px;
    text-align: center;
    padding: 2rem 0;
  }
  padding: 10px;
  .plano {
    border-radius: 10px;
    margin-bottom: 3rem;
    padding: 3rem 1rem;
    display: flex;
    flex-direction: column;
    align-items: center;
    h2 {
      font-size: 35px;
      text-align: center;
    }
    &.bg1 {
      background: #dbeafe;
    }
    &.bg2 {
      background: #f3f4f6;
    }
    h3 {
      font-size: 30px;
      text-align: center;
      padding: 10px 0;
      span {
        font-weight: 400;
        font-size: 15px;
      }
    }
    .subtitle {
      text-align: center;
    }

    .body {
      display: flex;
      .features {
        .feature {
          display: flex;
          align-items: center;
          justify-content: flex-end;
          min-height: 40px;
          padding-right: 10px;
          p {
            text-align: end;
            font-weight: 700;
            font-size: 12px;
          }
        }
      }
      .values {
        .value {
          display: flex;
          align-items: center;
          min-height: 40px;
          padding-left: 10px;

          .btn-increase {
            background: white;
            border: none;
            padding: 0px 15px;
            border-radius: 3px;
            font-weight: 700;
            font-size: 20px;
          }
          .field {
            padding: 0 10px;
          }
        }
      }
    }
    .btnspace {
      padding: 20px 0;
      text-align: center;
    }
  }
  @media only screen and (min-width: 1200px) {
    padding: 5rem 10rem;
  }
}
</style>
