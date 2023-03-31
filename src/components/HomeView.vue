/* eslint-disable */ to ignore all warnings in a file.
<template>
  <div class="container">
    <div class="first-section">
      <img src="@/assets/img/logopng.png" class="img">
      <div style="display: flex; flex-direction: column"> 
        <h4>
          Ajudamos empresas a venderem pela internet desde 2020.
        </h4>
          <ButtonVue @click="whatsAppTheo() || whatsAppRilson()" class="button" text="Quero vender pela internet!"/>
      </div>
    
    </div>
    </div>
</template>

<script>
import ButtonVue from './Button.vue';
// import Swal from "sweetalert2"
export default {
  components: {
    ButtonVue
  },
  setup() {
    async function whatsAppTheo(){
    //  await Swal.fire({
    //   icon: "success",
    //   title: "Aguarde!",
    //   text: "Você será levado ao WhatsApp!",
    //   background: "#2f2f2f",
    //   iconColor: "white",
    //   color: "white"
    //  });
       window.open("https://api.whatsapp.com/send?phone=5521967543780") 
    }
    function whatsAppRilson(){
       window.open("https://api.whatsapp.com/send?phone=5521999431819") 
    }
    return{
        whatsAppTheo,
        whatsAppRilson
    }
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
  background-size: auto;
}
.first-section {
  position: absolute;
  height: 400px;
  width: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  margin-top: -20vh;

}

.button{
  position: relative;
  margin-top: 5vh;
}
.img{
  margin-top: 4rem;
  padding: 20px;
  transform: scale(0.6);
  transition: transform 0.6s;
  transform-style: preserve-3d;
}
.img:hover{
  /* transform: rotateY(180deg); */
  transform: scale(0.8);

}
h4{
  /* padding: 10px; */
  position: relative;
  color: white;
  margin-bottom: -10vh;
  text-shadow: 2px 2px 0px rgb(161,0,242, .8);
}
@media screen and (max-height: 722px){
.img{
  margin-top: 2rem;
}
}

@media screen and (max-width: 700px) and (max-height: 900px){
  .container {
  display: flex;
  flex-direction: column;
  justify-content: center;
  width: 100%;
  height: 400px;
  background-image: url("@/assets/img/backgroundheader.jpg");
  background-repeat: no-repeat;
  background-size: auto;
  background-position-x: -350px;
}
}
@media only screen and (max-height: 900px){
  .container {
  display: flex;
  flex-direction: column;
  justify-content: center;
  width: 100%;
  height: 400px;
  background-image: url("@/assets/img/backgroundheader.jpg");
  background-repeat: no-repeat;
  background-size: auto;
  /* background-position-x: -350px; */
}
.img{
  transform: scale(0.4);
  float: left;
  margin-bottom: 0vh;
  position: absolute
}
h4{
  padding: 10px;
  position: relative;
  margin-top: 40vh;
  margin-bottom: 0vh;

  color: white;
  margin-bottom: 0vh;
  text-shadow: 2px 2px 0px rgb(161,0,242, .8);
}
.button{
  position: relative;
  margin-top: 5vh;
}
}
</style>
