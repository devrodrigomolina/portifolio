<template>
  <div class="header">
    <a class="logo" href="#home"><span>&lt;</span> Rodrigo Desenvolvedor <span>/&gt;</span></a>
    <ButtonsHeader/>
  </div>
</template>

<script>
import ButtonsHeader from "@/components/ButtonsHeader.vue"
export default {
  name: 'Header',
  components: {
    ButtonsHeader
  }
}
</script>

<style lang="scss" scoped>
.header {
  display: flex;
  align-items: center;
  position: fixed;
  z-index: 1001;
  justify-content: space-between;
  width: 100%;
  height: 60px;
  background: #060e1363;
  border-bottom: 1px solid #ffffff6b;
  .logo {
    color: white;
    font-size: 2rem;
    padding-left: 15px;
    transition: all .3s;
    &:hover {
      color: rgba(146, 145, 145, 0.842);
    }
    span {
      color: red;
    }
  }
}

@media (max-width: 560px) {
  .header {
    width: 100vw;
    height: 60px;
    z-index: 100;
    position: fixed;
    background: #060e1363;
    border-bottom: 1px solid #ffffff6b;
    .logo {
      color: white;
      font-size: 10px;
   
      transition: all .3s;
    }
  }
}
</style>

