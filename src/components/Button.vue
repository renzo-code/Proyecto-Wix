<template>
  <div>
    <button
      :class="['button', styles,classe]">
      {{ name }}
    </button>
  </div>
</template>

<script>
export default {
  name: 'Button',
  props: {
    name: String,
    styles: String,
    classe: String,
  },
}
</script>

<style lang="scss">
.button{
  padding: 12px 30px;
  border: none;
  font-size: 18px;
  background-color: #6EA4CA;
  color: white;
  cursor: pointer;
  &:hover{
    transition: 0.5s;
    color: #0C3C60;
  }
}
.btn-enviar{
margin-top: 20px;
margin-left: 238px;
}
.btn-saber-mas{
  background-color: #0C3C60;
  
  &:hover{
    transition: 0.5s;
    color: white;
    background-color: #39729B;
  }
}
</style>