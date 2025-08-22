<template>
  <div class="navMenu">
    <div class="webNavGroup">
      <a href="#home">HOME</a>
      <a href="#premios">PRÊMIOS</a>
      <a href="#comoParticipar">COMO PARTICIPAR</a>
      <a href="#ranking">RANKING</a>
      <div class="cta">
        <a href="#cta">PARTICIPE</a>
      </div>
    </div>
    <div class="mobileNavGroup">
      <img src="../assets/material/logo-mobile.png" alt="" height="50" />
      <img
        @click="toggleModal"
        class="navButton"
        src="../assets/material/menu-mobile.png"
        alt=""
        height="20"
      />
    </div>
  </div>
  <div v-if="isModal" class="modal">
    <a @click="toggleModal" href="#home">HOME</a>
    <a @click="toggleModal" href="#premios">PRÊMIOS</a>
    <a @click="toggleModal" href="#comoParticipar">COMO PARTICIPAR</a>
    <a @click="toggleModal" href="#ranking">RANKING</a>
    <a @click="toggleModal" href="#cta">PARTICIPE</a>
  </div>
</template>

<script lang="ts" setup>
import { ref } from 'vue'
const isModal = ref(false)

const toggleModal = () => {
  isModal.value = !isModal.value
}
</script>

<style>
.navMenu {
  width: 100%;
  display: flex;
  background-color: var(--yellow);
  font-weight: bold;
  justify-content: center;

  a {
    color: var(--blue);
  }
  @media (hover: hover) {
    a:hover {
      color: var(--yellow);
      background-color: var(--blue);
    }
  }
}

.webNavGroup {
  flex: content;
  display: flex;
  justify-content: space-around;
  justify-items: center;
  max-width: 1200px;
  a {
    padding: 1em;
  }
}

.mobileNavGroup {
  display: none;
}

.modal {
  display: none;
}

.cta a {
  display: flex;
  color: var(--yellow);
  background-color: var(--blue);
}

@media (max-width: 920px) {
  .webNavGroup {
    display: none;
  }

  .mobileNavGroup {
    padding: 0.5em;
    display: flex;
    justify-content: center;
    align-items: center;
  }

  .navButton {
    position: absolute;
    right: 30px;
  }

  .modal {
    width: 100%;
    font-size: 1em;
    display: flex;
    flex-direction: column;
    background-color: var(--blue);
    font-weight: bold;
    align-items: center;

    a {
      color: var(--yellow);
      padding: 0.5em;
    }
  }
}
</style>
