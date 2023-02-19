<template>
  <div class="planos" id="design">
    <h2 class="plan-title">Confira os planos</h2>
    <div class="plano">
      <h2 class="bg2">First Impression</h2>
      <h3>R$ 259,00/mês</h3>
      <div class="body">
        <div class="features">
          <div class="feature"><p>Posts no Feed</p></div>
          <div class="feature"><p>Versão Story</p></div>
          <div class="feature"><p>Agendamento de Posts</p></div>
          <div class="feature"><p>Elaboração do contéudo</p></div>
          <div class="feature"><p>Página de Link na Bio</p></div>
          <div class="feature"><p>Suporte</p></div>
        </div>
        <div class="values">
          <div class="value"><p>12 por mês</p></div>
          <div class="value"><p>05 por mês</p></div>
          <div class="value"><p>Sim</p></div>
          <div class="value"><p>Sim</p></div>
          <div class="value"><p>Não incluso</p></div>
          <div class="value"><p>Sim Via WhatsApp</p></div>
        </div>
      </div>
      <div class="btnspace">
        <a href="#" class="linkbtn">Quero saber mais</a>
      </div>
    </div>
    <div class="plano">
      <h2 class="bg1">Brand Booster</h2>
      <h3>R$ 399,00/mês</h3>
      <div class="body">
        <div class="features">
          <div class="feature"><p>Posts no Feed</p></div>
          <div class="feature"><p>Versão Story</p></div>

          <div class="feature"><p>Agendamento de Posts</p></div>
          <div class="feature"><p>Elaboração do contéudo</p></div>
          <div class="feature"><p>Página de Link na Bio</p></div>
          <div class="feature"><p>Suporte</p></div>
        </div>
        <div class="values">
          <div class="value"><p>17 por mês</p></div>
          <div class="value"><p>10 por mês</p></div>
          <div class="value"><p>Sim</p></div>
          <div class="value"><p>Sim</p></div>
          <div class="value"><p>Sim</p></div>
          <div class="value"><p>Via WhatsApp</p></div>
        </div>
      </div>
      <div class="btnspace">
        <a href="#" class="linkbtn">Quero saber mais</a>
      </div>
    </div>
    <div class="plano">
      <h2 class="bg3">Made on demand</h2>
      <h3>{{ customPreco }}/mês</h3>
      <p class="subtitle">
        Costumize seu plano conforme a necessidade do seu empreendimento.
      </p>
      <div class="body">
        <div class="features">
          <div class="feature"><p>Posts no Feed</p></div>
          <div class="feature"><p>Versão Story</p></div>

          <div class="feature"><p>Agendamento de Posts</p></div>
          <div class="feature"><p>Elaboração do contéudo</p></div>
          <div class="feature"><p>Página de Link na Bio</p></div>
          <div class="feature"><p>Suporte</p></div>
        </div>
        <div class="values">
          <div class="value">
            <button
              @click="qtd.posts > 0 ? qtd.posts-- : qtd.posts"
              class="btn"
            >
              -</button
            ><span class="field">{{ qtd.posts }}</span
            ><button @click="qtd.posts++" class="btn">+</button>
          </div>
          <div class="value">
            <button
              @click="qtd.stories > 0 ? qtd.stories-- : qtd.stories"
              class="btn"
            >
              -</button
            ><span class="field">{{ qtd.stories }}</span
            ><button @click="qtd.stories++" class="btn">+</button>
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
            <input type="checkbox" v-model="qtd.cardbio" id="cardbio" /><label
              for="cardbio"
              >cardbio</label
            >
          </div>

          <div class="value">
            <p>Via WhatsApp</p>
          </div>
        </div>
      </div>
      <div class="btnspace">
        <a href="#" class="linkbtn">Quero saber mais</a>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
export default {
  data: function () {
    return {
      qtd: {
        posts: 15,
        stories: 0,
        agendamento: false,
        conteudo: false,
        cardbio: false,
      },
    };
  },
  computed: {
    customPreco: function () {
      let preco = 0;
      let qtd = this.qtd;
      if (qtd.posts) {
        preco += qtd.posts * 12;
      }

      if (qtd.stories) {
        preco += qtd.stories * 5;
      }

      if (qtd.agendamento) {
        preco += 30;
      }

      if (qtd.conteudo) {
        preco += qtd.posts * 5;
      }

      if (qtd.cardbio) {
        preco += 30;
      }
      return preco.toLocaleString("pt-br", {
        style: "currency",
        currency: "BRL",
      });
    },
  },
};
</script>

<style lang="scss">
.planos {
  h2 {
    font-size: 40px;
    color: #f6f6f6;
    text-align: center;
    padding: 30px 0;
  }
  padding: 10px;
  .plano {
    border-radius: 10px;
    background: white;
    margin-bottom: 10px;
    padding: 10px;
    h2 {
      font-size: 50px;
      text-align: center;
      color: #f6f6f6;
      background-color: #32186f;
      padding: 5px;
      border-radius: 10px;
      &.bg1 {
        background-image: url("./assets/bg-05.jpg");
        background-size: cover;
      }
      &.bg2 {
        background-image: url("./assets/bg-06.jpg");
        background-size: cover;
      }
      &.bg3 {
        background-image: url("./assets/bg-07.jpg");
        background-size: cover;
      }
    }
    h3 {
      text-align: center;
      padding: 30px 0;
      font-weight: 400;
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
          .btn {
            background: #dfdfdf;
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
      .linkbtn {
        padding: 10px;
        color: white;
        text-decoration: none;
        font-size: 20px;
        background: #25d366;
        border-radius: 5px;
      }
    }
  }
}
</style>
