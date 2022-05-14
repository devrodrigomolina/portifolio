<template>
  <div id="app">
    <Header/>
    <Home/>
    <Sobre/>
    <Contato/>
    <Projetos/>
  </div>
</template>
<script>

import Header from "@/components/Header.vue";
import Home from "@/views/Home.vue";
import Contato from "@/views/Contato.vue";
import Sobre from "@/views/Sobre.vue";
import Projetos from "@/views/Projetos.vue";

export default {
  components: {
    Header,
    Home,
    Sobre,
    Contato,
    Projetos
  }
}
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Epilogue:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}
html {
  scroll-behavior: smooth;
  overflow-x: hidden;
}
body {
  font-family: 'Epilogue', sans-serif;
}
#app {
  display: flex;
  height: 100vh;
}
li {
  list-style: none;
}
a {
  text-decoration: none;
}
.btn {
  position: relative;
  padding: 10px 1.3em;
  border: none;
  background-color: transparent;
  cursor: pointer;
  outline: none;
  font-size: 16px;
  margin-right: 40px;
  &::after, &::before {
    content: '';
    display: block;
    position: absolute;
    width: 20%;
    height: 20%;
    border: 2px solid;
    transition: all 0.6s ease;
    border-radius: 2px;
  }
  &::after {
    bottom: 0;
    right: 0;
    border-top-color: transparent;
    border-left-color: transparent;
    border-bottom-color: white;
    border-right-color: white;
  }
  &::before {
    top: 0;
    left: 0;
    border-bottom-color: transparent;
    border-right-color: transparent;
    border-top-color: red;
    border-left-color: red;
  }
  &:hover:after, &:hover:before {
    width: 100%;
    height: 100%;
  }
}
@media (max-width: 360px) {
  .btn {
    padding: 5px 1rem;
    font-size: 10px;
    margin-right: 10px;
  }
}
</style>
