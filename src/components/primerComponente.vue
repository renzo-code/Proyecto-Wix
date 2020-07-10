<template>
  <div class="block">
    <h1 class="title" >{{ title }}</h1>
    <p class="parrafo">
      {{ parrafo }}
    </p>
  <Button name="Saber más"/>
  </div>
</template>

<script>
import Button from './Button'

export default {
  name: 'Block',
  props: {
    parrafo: String,
    title: String,
  },
  components:{ 
    Button,
  }

}
</script>

<style lang="scss">
.block{
  display: flex;
  flex-direction: column;
  background-color: #0C3C60;
  width: 300px;
  min-height: 400px;
  color: white;
  text-align: center;
  padding: 40px 20px;
}
.title{
  font-family: 'Raleway', sans-serif;
  font-weight: 600;
  font-size: 27px;
}
.parrafo{
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  padding-top: 25px;
  padding-bottom: 20px;
}

@media (max-width: 600px) {
  .block {
    width: 100%;
  }
}
</style>