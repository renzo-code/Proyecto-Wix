<template>
  <div class="feed">
    <h1 class="feed-item-title">CONTÁCTANOS</h1>
    <div class="contac">
      <div class="content">
        <iframe class="map" src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d6561.293037998583!2d-76.98111198308015!3d-12.086927870076341!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x9105c79f5dacafbf%3A0x2aecf92fd4325f0d!2sJockey%20Plaza!5e0!3m2!1ses-419!2spe!4v1594142495586!5m2!1ses-419!2spe" width="600" height="450" frameborder="0" style="border:0;" allowfullscreen="" aria-hidden="false" tabindex="0"></iframe>
        <div class="form">
          <h2 class="contac-item">
            Av. Los Rosales 122
            28021, Madrid
            info@misitio.com
            Tel: 914-123-456
          </h2>
          <div class="input-text">
            <InputText placeholder="Nombre"/>
            <InputText placeholder="Email"/>
            <InputText placeholder="Telefono"/>
            <AreaText />
            <Button styles="btn-enviar" name="Enviar"/>
          </div>
        </div>
      </div>
    </div>
    <div class="copyright">
      <h2 >© 2023 de Jaime Consultoría. Creado con Wix.com</h2>
      <div>
        <img class="icons-fb" src="https://static.wixstatic.com/media/7355b116f509973815da125ab3ce4065.wix_mp/v1/fill/w_24,h_24,al_c,usm_0.66_1.00_0.01/7355b116f509973815da125ab3ce4065.wix_mp">
        <img class="icons-fb" src="https://static.wixstatic.com/media/89b1d2497b29ccbb7d37be1ec6ef0052.png/v1/fill/w_25,h_24,al_c,q_85,usm_0.66_1.00_0.01/89b1d2497b29ccbb7d37be1ec6ef0052.webp">
      </div>
    </div>
  </div>
</template>

<script>
import InputText from '../components/InputText'
import AreaText from '../components/AreaText'
import Button from '../components/Button'

export default {
  name: 'Feed',
  components:{
    InputText,
    AreaText,
    Button
  }
}
</script>

<style lang="scss">
.feed{
  background-color: #0C3C60;
  min-height: 1050px;
  width: 100%;
}
.feed-item-title{
  padding: 90px 0 80px;
  color: white;
  font-family: 'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande', 'Lucida Sans', Arial, sans-serif;
  font-weight: 100;
  text-align: center;
  font-size: 70px;
}
.contac{
  width: 100%;
  & > .content {
    display: flex;
    justify-content: space-evenly;
    width: auto;
  }
}

.contac-item{
  padding-left: 75px;
  padding-right: 95px;
  margin-bottom: 15px;
}
.form{
  color: white;
  font-family: 'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande', 'Lucida Sans', Arial, sans-serif;
  font-weight: 100;
  font-size: 12px;
  text-align: center;
  width: 350px;
  margin-left: 70px;
}
.input-text{
  height: 375px;
  width: 350px;
}
.copyright{
  margin-top: 250px;
  color: white;
  font-weight: 100;
  font-family: 'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande', 'Lucida Sans', Arial, sans-serif;
  font-size: 10px;
  display: flex;
  justify-content: space-evenly;
}
.icons-fb{
  margin-right: 20px;
  cursor: pointer;
  height: 20px;
}

@media (max-width: 600px) {
  .contac {
    display: block;
    padding: 0;
    & > iframe {
      width: 100%;
    }
    & > .form {
      width: 100%;
      margin: 0;
      & > h2 {
        padding: 0 50px;
      }
      & > .input-text {
        width: 100%;
        padding: 0 10px;
      }
    }
  }
}
</style>