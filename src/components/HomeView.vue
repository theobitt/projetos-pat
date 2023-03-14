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
@media only screen and (max-width: 1024px) and (max-height: 768px){
  .container {
  display: flex;
  flex-direction: column;
  justify-content: center;
  width: 100%;
  height: 400px;
  background-image: url("@/assets/img/backgroundheader.jpg");
  background-repeat: no-repeat;
  background-size: 200%;
  background-position-x: -350px;
}
}
</style>
