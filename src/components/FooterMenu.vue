<template>
  <div class="footer">
    <div class="laco">
      <div class="whiteLine"></div>
      <img src="./../assets/material/footer/laco.png" />
      <div class="whiteLine"></div>
    </div>
    <div class="spaceBetween">
      <a>DÚVIDAS</a>
      <a>REGULAMENTO</a>
    </div>
    <div class="spaceBetween">
      <img src="../assets/material/footer/redes-twitter.png" alt="redes-twitter" />
      <img src="../assets/material/footer/redes-facebook.png" alt="redes-facebook" />
      <img src="../assets/material/footer/redes-instagram.png" alt="redes-instagram" />
      <img src="../assets/material/footer/redes-yt.png" alt="redes-yt" />
    </div>
    <div class="textContent">
      <p>Esta promoção não é patrocinada, endossada nem administrada pela Epic Games, Inc.</p>

      <p>
        Ao participar deste evento, na extensão permitida pela lei aplicável, os participantes
        concordam em liberar e isentar a Epic Games, Inc., seus licenciadores, seus respectivos
        afiliados e funcionários, executivos, diretores, agentes, contratados e outros
        representantes de toda e qualquer reclamação, exigência, ação, perda, responsabilidade e
        despesa relacionada à promoção.
      </p>

      <p>
        As informações dos participantes fornecidas ligadas a esta promoção são entregues ao
        patrocinador, não a Epic Games, Inc.
      </p>

      <p>
        Participe de 11 a 25.11.24. Veja regulamento e Certificado de Autorização em
        loot-hellmanns.com.br. Imagens ilustrativas.
      </p>
    </div>
    <img src="../assets/material/footer/unilever.png" alt="" />
  </div>
</template>

<style scoped>
.footer {
  display: flex;
  flex-direction: column;
  align-items: center;
  background-color: var(--blue);
  color: white;
  gap: 1em;
  padding: 1em;
}

.whiteLine {
  height: 1px;
  width: 40%;
  border: solid 1px white;
}

.laco {
  width: 100%;
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
}

.spaceBetween {
  gap: 3em;
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
}

.textContent {
  max-width: 80%;
  text-align: center;
  font-family: sans-serif;
  font-size: 0.6em;
  line-height: 2;
}
</style>
