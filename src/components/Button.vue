<template>
  <div>
    <button class="button">{{ name }}</button>
  </div>
</template>

<script>
export default {
  name: 'Button',
  props: {
    name: String,
  }
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
</style>