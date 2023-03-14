/* eslint-disable */ to ignore all warnings in a file.
<template>
  <div class="container">
    <div class="first-section">
      <img src="@/assets/img/logopng.png" class="img">
      <div style="display: flex; flex-direction: column"> 
        <h4>
          Ajudamos empresas a venderem pela internet desde 2020.
        </h4>
        <ButtonVue class="button" text="Quero vender pela internet!"/>
      </div>
    
    </div>
    </div>
</template>

<script>
import ButtonVue from './Button.vue';
export default {
  components: {
    ButtonVue
  }
};
</script>

<style scoped>
.container {
  display: flex;
  flex-direction: column;
  justify-content: center;
  width: 100%;
  height: 400px;
  background-image: url("@/assets/img/backgroundheader.jpg");
  background-repeat: no-repeat;
  background-size: 100%;
}
.first-section {
  position: absolute;
  width: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  margin-top: -10vh;

}
.button{
  position: relative;
  margin-top: 5vh;
}
.img{
  transform: scale(0.5);
}
h4{
  padding: 10px;
  position: relative;
  color: white;
  margin-top: -10vh;
  text-shadow: 2px 2px 0px rgb(161,0,242, .8);

}
</style>
