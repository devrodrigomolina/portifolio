<template>
  <nav>  
    <a href="#sobre" class="btn">Sobre</a>
    <a href="#contato" class="btn">Contato</a>
    <a href="#projetos" class="btn">Projetos</a>
  </nav>
</template>

<script>
export default {
  name: "ButtonsHeader",
}
</script>

<style lang="scss" scoped>
nav {
  width: 300px;
  display: flex;
  justify-content: space-between;
  margin-right: 150px;
  a {
    color: white;
  }
}

@media (max-width: 360px) {
  nav {
    margin-left: 20px;
    width: auto;
  }
}
</style>