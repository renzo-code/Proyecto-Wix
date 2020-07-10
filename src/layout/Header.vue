<template>
  <header class="header">
    <h1 class="nombre">Jaime<span>Consultoría</span></h1>
    <div class="list">
      <label class="list-item" for="text">Sobre mí</label>
      <label class="list-item" for="text">Servicios</label>
      <label class="list-item" for="text">Proyectos</label>
      <label class="list-item" for="text">Clientes</label>
      <label class="list-item" for="text">Contacto</label>
    </div>
  </header>
</template>

<script>
export default {
  name: 'Header',
}
</script>

<style lang="scss">
.header{
  display: flex;
  justify-content: space-evenly;
  align-items: center;
  background-color: #0C3C60;
  font-size: medium;
  width: 100%;
  height: 89px;
}
.nombre {
  font-family: 'Raleway', sans-serif;
  color: white;
  & > span {
    color: #7BC7D8;
  }
}
.list-item:hover{
  opacity: 0.7;
  color: lightslategray;
}
.list-item{
  color: white;
  padding-right: 30px;
  cursor: pointer;
}
.list{
  font-family: 'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande', 'Lucida Sans', Arial, sans-serif;
}
</style>