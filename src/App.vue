<script setup>
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'
import Navi from './components/nav/Navi.vue'
import DataDiri from './components/komponen/DataDiri.vue'
import CardSkill from './components/komponen/CardSkill.vue'
import TitleSec from './components/komponen/TitleSec.vue'
import AboutMe from './components/komponen/AboutMe.vue'
import ProjectList from './components/komponen/ProjectList.vue'
import FooterV from './components/komponen/FooterV.vue'
</script>

<template>
  <header>
     <Navi />
  </header>
  <main>
    <DataDiri />
    
    <AboutMe />
    <TitleSec skill="SKILL"/>
    <CardSkill :cards="cards"/>
    <TitleSec skill="PROJECTS"/>
    <ProjectList />
  </main>
<FooterV />
  <RouterView />
</template>

<script>
export default{
  components: {Navi, DataDiri, CardSkill, TitleSec, AboutMe, ProjectList, FooterV},
  data() {
    return {
      cards: [
                {
                    title: 'Fullstack Developer',
                    image: '/icon/ic_web.png',
                },
                {
                    title: 'Game Developer',
                    image: '/icon/ic_game.png',
                },
                {
                    title: 'AR/VR Developer',
                    image: '/icon/ic_ar.png',
                },
            ]
    }
  },
}
</script>

<style scoped>
main {
  margin: 0 100px;
}
header {
  margin: 0 100px;
}

/* Responsive styles */
@media (max-width: 768px) {
  main {
    margin: 0 20px; /* Reduced margin for mobile */
  }
  
  header {
    margin: 0 20px; /* Reduced margin for mobile */
  }
}
</style>
