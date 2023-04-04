<template>
  <div class="main-container">
    <div class="context">
      <h2 id="projects" class="projects fs-1 p-1 m-0">Meus projetos</h2>
    </div>
    <div>
      <Cakes
        :cake="game1"
        name="Noite de fogo - 2022"
        link="https://kklavi.itch.io/noite-de-fogo"
        color="1"
        description="Um Jogo feito em uma gamejam de 48 horas, um endless runner frenético em que você controla o Boitatá e  caça lenhadores ilegais que estão desmatando a floresta amazônica"
      />
      <Cakes2
        :cake="game2"
        name="Vanishing Blade - 2022"
        link="https://jotapeoliveira.itch.io/vanishinblade"
        color="1"
        description="Em uma das minhas game jams eu e minha equipe criamos o Vanishing Blade, um jogo de plataforma side scroller onde um guerreiro amaldiçoado a quebrar toda a arma que usa"
      />
      <Cakes
      :cake="game3"
      name="RPG - medo do escuro - 2022"
      link="https://kklavi.itch.io/rpg-medo-do-escuro"
      color="1"
      description="Um RPG de mesa que crier na faculdade, onde um narrador controla o monstro do escuro e um jogador controla a criança que tentará superar seu medo"
    />
    <Cakes2
    :cake="game4"
    name="Manny rooms - 2022"
    link="https://kklavi.itch.io/manny-rooms"
    color="1"
    description="Um trabalho da faculdade que acabou se tornando um jogo, muito inspirado nas “backrooms” ele é um pequeno jogo de terror liminal"
  />
    </div>
  </div>
</template>

<script>

import Cakes from "./Cakes.vue";
import Cakes2 from "./Cakes2.vue";


import boloBrigadeiro from "../assets/imgs/cakes/bolo1.jpg";
import game1 from "../assets/game1.png"
import game2 from "../assets/game2.png"
import game3 from "../assets/game3.png"
import game4 from "../assets/game4.png"

export default {
  name: "Main",
  data() {
    return {
      game1: game1,
      game2: game2,
      game3: game3, 
      game4: game4
        
    };
  },
  components: {
    Cakes,
    Cakes2
  },
};
</script>

<style scoped>
.main-container {
  margin: 0 auto;
  max-width: 80vw;
  background: rgb(0, 0, 0);
}

.context {
  background: rgb(138, 138, 138);
  padding: 30px;
}


</style>