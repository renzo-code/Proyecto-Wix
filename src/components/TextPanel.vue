<template>
  <div class="panel">
    <div class="content">
      <h1 class="encabezado">Sobre Mí</h1>
      <p class="text">
        Párrafo. Haz clic para editar y agregar tu propio texto. Es fácil. Haz clic en 
        Editar Texto o doble clic aquí para agregar tu contenido y cambiar la fuente. 
        Puedes arrastrar y soltar este texto donde sea que quieras en tu página. 
        En este espacio puedes contar tu historia y permitir a tus usuarios saber más sobre ti.
        Este es un buen espacio para extenderte sobre tu compañía y servicios. 
        Puedes usar este espacio para incorporar más detalles sobre tu empresa. 
        Escribe sobre tu personal y los servicios que ofreces. Cuéntales a los visitantes 
        la historia sobre cómo se te ocurrió la idea de tu negocio y diles qué te diferencia de tus competidores. 
        Haz que tu empresa se destaque y muestra a tus visitantes quién eres.
      </p>
      <Button classe="btn-saber-mas" name="Saber más"/>
    </div>
  </div>
</template>

<script>
import Button from './Button'

export default {
  name: 'TextPanel',
  components:{
    Button,
  } 
}
</script>

<style lang="scss">
.panel{
  text-align: center;
  background-color: #D1E0EB;
  padding-top: 80px;
  color: #0C3C60;
  min-height: 500px;
  width: 100%;
}
.content {
  margin: 0 auto;
  width: 650px;
}

.encabezado{
  font-family: 'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande', 'Lucida Sans', Arial, sans-serif;
  font-size: 70px;
  font-weight: 100;
}
.text{
  /* margin: 50px 550px 70px; */
  font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
}

@media (max-width: 600px) {
  .panel {

  }
  .content {
    width: 100%;
    padding: 0 10px;
    & .btn-saber-mas {
      margin: 20px 0;
    }
  }
}
</style>