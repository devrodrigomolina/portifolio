<template>
  <div id="sobre" class="container">
    <Header/>
    <div class="container-infos">
      <div class="my-infos">
        <div class="foto">
          <img src="@/assets/eu.png" alt="">
        </div>
        <div class="infos">
          <h1 class="titulo">Sobre mim</h1>
          <h3>OLÁ !</h3> 
          <h2>EU SOU O <span>RODRIGO MOLINA</span></h2>
          <p>Olá, sou o Rodrigo tenho 29 anos, sou empresário no ramo de bicicletas e um amante da tecnologia, estou estudando Desenvolvimento web a 1,5 anos, Estou cursando Análise e Desenvolvimento de Sistemas, e estou em busca do meu primeiro emprego na área de Desenvolvimento..</p>
          <h1 class="titulo">Tecnologias</h1>
          <div class="techs">
            <div class="html">
              <img src="@/assets/html5.png" alt="">
              <p>HTML</p>
            </div>
            <div class="css">
              <img src="@/assets/css3.png" alt="">
              <p>CSS</p>
            </div>
            <div class="sass">
              <img src="@/assets/sass.png" alt="">
              <p>SASS</p>
            </div>
            <div class="js">
              <img src="@/assets/javascript.png" alt="">
              <p>JAVASCRIPT</p>
            </div>
            <div class="vue">
              <img src="@/assets/vue.png" alt="">
              <p>VUE.JS</p>
            </div>
          </div>
        </div>
    </div>
    </div>
  </div>

</template>

<script>


export default {
  name: "Sobre"
}
</script>

<style lang="scss" scoped>
.container {
  width: 100vw;
  height: 100vh;
  background-image: url("../assets/background3.jpg");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  .container-infos {
    width: 100vw;
    height: 100vh;
    display: flex;
    align-items: center;
    justify-content: center;
    background: rgba(0, 0, 0, 0.445); 
    .my-infos {
      width:1100px;
      height: 700px;
      display: flex;
      align-items: center;
      justify-content: center;
      background: rgba(255, 255, 255, 0.719);
      border-radius: 20px;
      .foto {
        margin: 60px;
        img {
          box-shadow: 1px 4px 8px rgba(0, 0, 0, 0.692);
          width: 300px;
          border-radius: 18px;
        }
      }
      .infos {
        width: 600px;
        height: 430px;
        .titulo {
          padding: 40px 0px;
          font-size: 20px;
          font-weight: 700;
          color: rgba(0, 0, 0, 0.473);
          &::after {
            content: ' →';    
          }
        }
        h2 {
          font-size: 2.5rem;
          margin-bottom: 15px;
          span {
            color: red;
          }
        }
        h3 {
          font-size: 1.5rem;
          color: rgba(0, 0, 0, 0.308);
        }
        p {
         
          color: rgba(0, 0, 0, 0.466);
          font-weight: 500;
          font-size: 18px;
          font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
          text-align: justify;
        }
        .techs {
          display: flex;
          align-items: center;
          justify-content: space-between;
          .html,.css,.js,.vue,.sass {
            transition: all .3s;
            p {
              text-align: center;
            }
            &:hover {
              transform: scale(1.1);
            }
          }
          img {
            margin: auto 20px;
          }
        }
      }
    }
  }
}

@media (max-width: 560px) {
.container {
  .container-infos {     
    .my-infos {
      width: 300px;
      height: 500px;
      display: flex;
      flex-direction: column;
      background: rgba(255, 255, 255, 0.719);
      border-radius: 20px;
      .foto {
        margin: 0;
        img {
          box-shadow: 1px 4px 8px rgba(0, 0, 0, 0.692);
          width: 100px;
          border-radius: 18px;
        }
      }
      .infos {
        width: 300px;
        height: 300px;
    
        .titulo {
          padding: 10px 10px 20px 10px;
        }
        h3 {
          font-size: 1rem;
          padding-left: 16px;
          color: rgba(0, 0, 0, 0.308);
        }
        h2 {
          text-align: center;
          font-size: 20px;
          span {
            color: red;
            font-size: 20px;
          }
        }
        p {
          color: rgba(0, 0, 0, 0.363);
          font-weight: 500;
          font-size: 10px;
          text-align: justify;
          margin: 16px;
        }
        .techs {
          margin-top: 8px;
          .html,.css,.js,.vue,.sass {
            display: flex;
            align-items: center;
            flex-direction: column;
            justify-content: space-between;
            transition: all .3s;
            p {
              text-align: center;
            }
            &:hover {
              transform: scale(1.1);
            }
          }
          img {
            width: 40px;
            margin: auto 0px;
          }
        }
      }
    }
  }
}
}

</style>