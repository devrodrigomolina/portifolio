<template>
  <div class="container-ctt" id="contato" >
  
    <Header/>
    <ul>
      <img src="../assets/github.png" alt="">
      <img src="../assets/linkedin.png" alt="">
      <img src="../assets/github.png" alt="">
      <img src="../assets/linkedin.png" alt="">
    </ul>
  </div>
</template>

<script>

export default {
  name: "Contato",

}
</script>

<style lang="scss" scoped>

.container-ctt {
  width: 100vw;
  height: 100vh;
  background-image: url("../assets/back2.jpg");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  ul {
    width: 100vw;
    height: 100vh;
    background: rgba(58, 58, 58, 0.247);
    display: flex;
    align-items: center;
    justify-content: center;
    img {
      margin-right: 30px;
      width: 140px;
      height: 140px;
      transition: all .3s;
      &:hover {
        transform: scale(1.1);
      }
    }
  }
}
@media (max-width: 560px) {
.container-ctt { 
  
    ul {
      img {
        margin-right: 30px;
        width: 40px;
        height: 40px;
        transition: all .3s;
     }
    }
  }
}
</style>