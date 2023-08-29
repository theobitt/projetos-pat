<template>
  <div class="home-container">
      <FirstSection id="first-section"/>
    <PurpleWidth id="purple"/>
      <ServicesSection id="servicos"/>
      <nossosClientes/>
      <about-us id="always"/>
      <FooterComponent />
  </div>
</template>

<script>
import FirstSection from '@/components/HomeView.vue'
import PurpleWidth from '@/components/PurpleWidth.vue'
import AboutUs from '@/components/AboutUs.vue'
import ServicesSection from '@/components/ServicesSection.vue'
import FooterComponent from '@/components/FooterComponent.vue'
import nossosClientes from '@/components/nossosClientes.vue'
// import VueWhatsappWidget from "vue-whatsapp-widget";


export default {
  // eslint-disable-next-line
  name: "Home",

  components:{
    FirstSection,
    PurpleWidth,
    AboutUs,
    ServicesSection,
    FooterComponent,
    nossosClientes
  }
}
</script>
<style scoped>

.home-container {
  display: flex;
  flex-direction: column;
  justify-content: center;
  width: 100%;
}
.navbar{
  justify-content: center;
  align-content: center;
  width: 100%;
  display: block;
  position: fixed;
  top: 1px;
  z-index: 3;
  
}
.nav-content{
  padding: 10px;
  background-color: rgba(0,0,0,0.4);
  border-radius: 1vh;
  width: 400px;
  gap: 1vh;
  /* justify-self: right; */
  /* position: absolute; */
  /* float: left; */
  display: flex;
}
.nav-link{
  text-decoration: none;
  color: white;
  font-size: 13px;
}
.nav-link:hover{
  cursor: pointer;
  color: var(--c-light)
}
.call-to-action-container {
  display: flex;
  justify-content: center;
  flex-direction: column;
  text-align: center;
  background-color: rgb(30, 30, 30);
  width: 100%;
  height: 400px;
  position: absolute;
}
h1 {
  text-shadow: 2px 2px 0px rgba(0,0,0,0.4);
}

.title-call-to-action {
  color: white;
  /* color: var(--c-light); */
}
.text-call-to-action{
  color: white;
  font-size: 15px;
}
.img-logo{
  width: 200px;
  height: 200px;
  margin-top: 15vh;
  /* transform: scale(0.6); */
  position: relative;
}
</style>