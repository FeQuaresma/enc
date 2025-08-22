<template>
  <div id="home"></div>
  <div class="mainBanner scrollMargin">
    <img class="mainLogo" src="../assets/material/home/logo-promo.webp" alt="logo-promo" />
  </div>

  <div class="mobileMainBanner scrollMargin">
    <img class="mainLogoMobile" src="../assets/material/home/logo-promo.webp" alt="logo-promo" />
    <img class="bgMobile" src="../assets/material/home/bg-home-mob.webp" alt="" />
  </div>
  <div>
    <div class="ballon1">
      <img src="../assets/material/premios/premios-balao-1.webp" alt="balao1" />
    </div>
    <div id="cta" class="textContent scrollMargin">
      <p>PARTICIPE DO <span>DESAFIO HELLMANN'S LOOT IRRESISTÍVEL</span></p>
      <p>E CONCORRA A PRÊMIOS ESPECIAIS</p>
      <button>PARTICIPE</button>
    </div>

    <div id="premios" class="prizesContent scrollMargin">
      <img
        class="webTitle"
        src="../assets/material/premios/titulo-premios.webp"
        alt="titulo-premios"
      />
      <img
        class="mobileTitle"
        src="../assets/material/premios/titulo-premios-mob.webp"
        alt="titulo-premios"
      />
      <div class="prizesBox">
        <img src="../assets/material/premios/premios-1.webp" alt="premio1" />
        <img src="../assets/material/premios/premios-2.webp" alt="premio2" />
        <img src="../assets/material/premios/premios-3.webp" alt="premio3" />
        <img src="../assets/material/premios/premios-4.webp" alt="premio4" />
      </div>
      <div class="ballon2">
        <img src="../assets/material/premios/premios-balao-2.webp" alt="balao2" />
      </div>
      <img
        class="scrollMargin"
        id="comoParticipar"
        src="../assets/material/como-participar/titulo-como-jogar.webp"
        alt="titulo-como-jogar"
        width="300px"
      />
      <div class="howToBox">
        <div>
          <img src="../assets/material/como-participar/como-participar-1.webp" alt="howTo1" />
          <img src="../assets/material/como-participar/como-participar-2.webp" alt="howTo2" />
          <img src="../assets/material/como-participar/como-participar-3.webp" alt="howTo3" />
        </div>
      </div>
      <div id="ranking" class="scrollMargin"></div>
      <img
        class="webTitle"
        src="../assets/material/como-participar/box-texto.webp"
        alt="box-texto"
      />
      <img
        class="mobileTitle"
        src="../assets/material/como-participar/box-texto-mob.webp"
        alt="box-texto"
      />
    </div>

    <div class="maioneseContent">
      <img class="maionese" src="../assets/material/como-participar/maionese.webp" alt="" />
      <div class="textContent">
        <p>GARANTA AQUI O SABOR IRRESISTÍVEL</p>
        <p>PARA A SUA GAMEPLAY</p>
        <button>COMPRE AGORA</button>
      </div>
      <img class="maionese" src="../assets/material/como-participar/maionese.webp" alt="" />
    </div>
  </div>
</template>

<style scoped>
.scrollMargin {
  scroll-margin-top: 60px;
}
.ballon1 {
  position: relative;
  height: 0;
  top: 10px;
  z-index: 100;
}

.mobileTitle {
  display: none;
}

.ballon2 {
  position: relative;
  height: 0;
  bottom: 280px;
  left: 550px;
  z-index: 101;

  img {
    height: 16em;
  }
}

.mainBanner {
  display: flex;
  background-image: url('../assets/material/home/bg-home.webp');
  background-position: center;
  background-repeat: no-repeat;
  background-color: var(--marine-blue);
  min-height: 600px;
  background-size: auto 100%;
  justify-content: center;

  img {
    max-height: 550px;
    margin-right: 150px;
  }
}

.textContent {
  padding: 1em;
  font-size: 1.5em;
  font-weight: bold;
  color: var(--blue);
  text-align: center;
  span {
    color: var(--marine-blue);
  }
}

.prizesContent {
  background-image: url('../assets/material/premios/bg-premios.webp');
  background-position: top center;
  background-color: var(--marine-blue);
  background-size: 100%;
  background-repeat: no-repeat;
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 2em;
}

.prizesBox {
  margin: 2em;
  margin-bottom: 4em;
  display: flex;
  flex-wrap: wrap;
  max-width: 1200px;
  justify-content: center;
}

.howToBox {
  margin: 1.5em 0.2em;
  border-radius: 1em;
  background-color: var(--yellow);

  div {
    margin: 1em;
    border: solid 2px var(--blue);
    border-radius: 1em;
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
  }

  img {
    margin: 1em;
  }
}

.maioneseContent {
  padding: 1em 0;
  display: flex;
  justify-content: center;

  img {
    height: 150px;
  }
}

.mobileMainBanner {
  display: none;
}
@media (max-width: 1307px) {
  .ballon2 {
    left: 250px;
  }
}
@media (max-width: 1080px) {
  .mainBanner {
    min-height: 500px;
    img {
      max-height: 450px;
    }
  }
}
@media (max-width: 920px) {
  .ballon1,
  .ballon2,
  .maionese,
  .webTitle,
  .mainBanner {
    display: none;
  }

  .scrollMargin {
    scroll-margin-top: 70px;
  }
  .mobileTitle {
    display: block;
  }

  .mobileMainBanner {
    display: flex;
    justify-content: center;

    .mainLogoMobile {
      position: absolute;
    }

    .bgMobile {
      width: 100vw;
      max-height: 92vh;
      object-fit: cover;
      object-position: bottom;
    }
  }

  .prizesBox {
    margin: 1em 0;

    img {
      max-width: 100%;
    }
  }

  .prizesContent {
    padding: 1em 0.2em;
    background-image: url('../assets/material/premios/bg-premios-mob.webp');
  }
  .textContent {
    font-size: 1.5em;
  }
}
</style>
