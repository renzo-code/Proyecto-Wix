<template>
  <div class="input-padre">
    <input :placeholder="placeholder" class="input-texto" type="text">
  </div>
</template>

<script>
export default {
  name:'InputText',
  props:{
    placeholder: String,
  }
}
</script>

<style lang="scss">
.input-padre{
  height: 15px;
  padding-top: 30px;
  margin-bottom: 15px; 
}
.input-texto{
  width: 100%;
  height: 35px;
  padding-left: 20px;
  font-size: 15px;
  outline: none;
  &:hover{
    transition: 0.2s;
    border: solid 2px #6EA4CA;
  }
}
</style>