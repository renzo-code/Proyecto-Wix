<template>
  <div class="text-area">
    <textarea class="text-area-item" cols="30" placeholder="Escribe tú mensaje aquí..."></textarea>
  </div>
</template>

<script>
export default {
  name: 'AreaText'
}
</script>

<style lang="scss">
.text-area-item{
  height: 118px;
  width: 100%;
  text-align: top;
  font-family: 'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande', 'Lucida Sans', Arial, sans-serif;
  font-size: 15px;
  padding-left: 20px;
  padding-top: 10px;
  outline: none;
  &:hover{
    transition: 0.2s;
    border: solid 2px #6EA4CA;
  }
}
.text-area{
  margin-top: 45px;
}
</style>