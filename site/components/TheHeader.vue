<template>
  <div class="header">
    <div class="center">
      <img class="logo" src="@/assets/logo-branca.svg" />
    </div>
    <div class="text">
      <h3>
        Redes sociais e design para <span>{{ nicho }}</span>
      </h3>
      <p>Eu vou te ajudar a melhorar sua presença no mundo digital!</p>
    </div>
    <div class="center">
      <a class="btn btn-dark" href="#">Agendar um contato</a>
    </div>
  </div>
</template>

<script lang="ts">
export default {
  data: function () {
    return {
      nicho: "Esteticistas",
      nichos: [
        "Academia",
        "Arquiteto",
        "Barbearia",
        "Boutique",
        "Cafeteria",
        "Contador",
        "Corretor",
        "Creche",
        "Delivery",
        "Doceria",
        "E-commerce",
        "Estética",
        "Eventos",
        "Farmácia",
        "Hamburgueria",
        "Hotel",
        "Lava-rápido",
        "Médico",
        "Nutricionista",
        "Odontologia",
        "Oficina",
        "Papelaria",
        "Pet shop",
        "Pizzaria",
        "Psicólogo",
        "Restaurante",
        "Supermercado",
      ],
    };
  },
  mounted() {
    setInterval(() => {
      const index = Math.floor(Math.random() * this.nichos.length);
      this.nicho = this.nichos[index];
    }, 3000);
  },
};
</script>

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
