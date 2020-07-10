<template>
  <div id="app">
    <Header />
    <div class="image-index">
      <img src="https://static.wixstatic.com/media/84770f_573f9ee905a043e18a65f49e31c1c7e8.jpg/v1/fill/w_1903,h_754,al_t,q_85,usm_0.66_1.00_0.01/84770f_573f9ee905a043e18a65f49e31c1c7e8.webp">    
    </div>
    <div class="blocked">
      <Block :parrafo="parrafo" title="Servicio" />
      <Block :parrafo="parrafo" title="Proyectos" />
      <Block :parrafo="parrafo" title="Clientes" />
    </div>
    <TextPanel />
    <Feed />
  </div>
</template>

<script>
import Header from './layout/Header'
import Block from './components/primerComponente'
import TextPanel from './components/TextPanel'
import Feed from './layout/Feed'

export default {
  name: 'App',
  components: {
    Header,
    Block,
    TextPanel,
    Feed,
  },
  data() {
    return {
      parrafo: 'Este es un buen espacio para extenderte sobre tu compañía y servicios. Puedes usar este espacio para incorporar más detalles sobre tu empresa. Escribe sobre tu personal y los servicios que ofreces. Cuéntales a los visitantes la historia sobre cómo se te ocurrió la idea de tu negocio y diles qué te diferencia de tus competidores. ',
    }
  }
}
</script>

<style lang="scss">
*{
  box-sizing: border-box;
  padding: 0;
  margin: 0;
}
.image-index {
  height: 685px;
  width: 100%;
  & > img {
    width: 100%;
    height: 100%;
    object-fit: cover;
  }
}
.blocked{
  display: flex;
  justify-content: space-evenly;
  padding: 75px 420px;
}
</style>
