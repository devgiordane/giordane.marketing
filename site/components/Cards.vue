<template>
  <div class="cards">
    <div class="card bg-1">
      <img src="@/assets/el-01.png" class="el-1" />
      <h3>Social Media</h3>
      <p>
        Além de vídeos imagens e carrosseis, levamos estratégia e credibilidade
        para sua marca!
      </p>
      <a class="btn btn-white" href="#design">Saiba mais</a>
    </div>
    <div class="card bg-2">
      <img src="@/assets/el-02.png" class="el-2" />
      <h3 class="game pt">KIT START SOCIAL</h3>
      <p>
        Um combo para pequenos empreendedores terem uma base sólida para sua
        marca.
      </p>
      <a class="btn btn-white" href="#kit">Saiba mais</a>
    </div>
    <div class="card bg-3">
      <img src="@/assets/el-03.png" class="el-1" />
      <h3 class="pt">Identidade Visual</h3>
      <p>
        Vamos dar vida a sua ideia e trazer personalidade para o seu négocio.
      </p>
      <a class="btn btn-white" href="#identidade">Saiba mais</a>
    </div>
  </div>
</template>

<style lang="scss">
.cards {
  padding: 5rem 1rem;

  .card {
    .el-1 {
      position: absolute;
      max-width: 100px;
      left: -10px;
      top: -30px;
    }
    .el-2 {
      position: absolute;
      max-width: 100px;
      right: -10px;
      top: -30px;
    }

    position: relative;
    color: white;
    display: flex;
    flex-direction: column;
    justify-content: space-evenly;
    align-items: center;
    text-align: center;
    border-radius: 10px;
    padding-top: 5rem;
    min-height: 330px;
    &:not(:last-child) {
      margin-bottom: 3rem;
    }
    &.bg-1 {
      background-image: url("./assets/bg-01.jpg");
      background-size: cover;
    }
    &.bg-3 {
      background-image: url("./assets/bg-03.jpg");
      background-size: cover;
    }
    &.bg-2 {
      background-image: linear-gradient(to right, #833ab4, #fd1d1d, #fcb045);
      background-size: cover;
    }
    h3 {
      font-size: 38px;
      &.game {
        font-family: "Press Start 2P", cursive;
        font-size: 22px;
      }
    }
  }
}
</style>
