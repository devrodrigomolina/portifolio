<template>
  <div id="home" class="home">
    <Header/>
    <div class="container-infos">
      <div class="infos">
        <h2 class="hello">Hello World, eu sou o</h2>
        <h1>Rodrigo Molina</h1>
        <h2 class="skill-info">DESENVOLVEDOR FRONT-END</h2>
      </div>
    </div>

  </div>
</template>

<script>
import Sobre from "@/views/Sobre.vue"
import Contato from "@/views/Contato.vue"


export default {
  name: 'Home',
  components: {
    Sobre,
    Contato
  }
}
</script>

<style scoped lang="scss">
.home {
  width: 100vw;
  height: 100vh;
  background-image: url("../assets/background2.jpg");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  .container-infos {
    width: 100vw;
    height: 100vh;
    display: flex;
    align-items: center;
    padding-left: 100px;

    .infos {
      width: 610px;
      .hello {
        text-transform: uppercase;
        font-size: 2rem;
        color: rgba(170, 168, 168, 0.363);
      }
      h1 {
        margin: 5px 0;
        color: white;
        font-size: 5rem;
      }
      .skill-info {
        padding-left: 330px;
        font-size: 1.2rem;
        color: rgba(255, 0, 0, 0.425);
      }
    }
  }
}

@media (max-width: 560px) {
.home {
  width: 100vw;
  height: 100vh;
  background-image: url("../assets/background2.jpg");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  .container-infos { 
    width: 100vw;
    height: 100vh;
    background: rgba(0, 0, 0, 0.541);
    display: flex;
    align-items: center;
    padding-left: 10px;
    .infos {
      padding-top: 120px;
      .hello {
        text-transform: uppercase;
        font-size: 1rem;
        color: rgba(170, 168, 168, 0.363);
      }
      h1 {
        margin: 5px 0;
        color: white;
        font-size: 2rem;
      }
      .skill-info {
        padding-left: 55px;
        font-size: 13px;
        color: rgba(255, 0, 0, 0.425);
      }
    }
  }
}
}

</style>