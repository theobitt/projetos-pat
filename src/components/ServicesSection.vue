/* eslint-disable */
<template>
  <div class="services-container">
    <div class="title">
      <h1 style="color: white;">Como podemos te ajudar?</h1>
    </div>
    <div class="service-row">
      <div class="each-box">
        <h1>Tráfego pago</h1>
        Aumente suas vendas com o nosso serviço de anúncios nas plataformas do
        Google, YouTube, Facebook e Instagram.
      </div>
      <div class="each-box">
        <h1>Social Media</h1>
        Aumente sua presença nas redes sociais com o nosso serviço de
        <a style="color: var(--c-default)"> Social Media. </a>
      </div>
    </div>
    <div class="service-row">
      <div class="each-box">
        <h1>Landing Pages</h1>
        Venda seu produto ou serviço em uma única página na Internet!
        <p>
          Chega de sites lotados de informação que mais
          <a style="color: var(--c-default)"> confundem do que convertem. </a>
        </p>
      </div>
      <div class="each-box">
        <h1>Design</h1>
        Tenha um visual <a style="color: var(--c-default)"> único </a> para sua
        empresa com nosso serviço de criação de identidade visual!
      </div>
    </div>

    <div class="service-row"></div>
  </div>
</template>

<script>
export default {
  name: "ServicesSection",
};
</script>

<style scoped>
.services-container {
  display: flex;
  flex-direction: column;
  justify-content: center;
  background: linear-gradient(52deg, rgb(40, 34, 34) 20%, rgb(54, 54, 54) 100%);
  width: 100%;
  height: auto;
  gap: 15vh;
}
.service-row {
  gap: 25vh;
  display: flex;
  flex-direction: row;
  justify-content: center;
}
.each-box {
  padding: 15px;
  border: 3px solid var(--c-default);
  transition: transform 0.6s;
  transform-style: preserve-3d;
  background-color: var(--c-cleangrey2);
  width: 350px;
  height: 200px;
  font-weight: bold;
  border-radius: 20px;
  text-decoration-line: none; 
  color: white;
}
.each-box:hover {
  transform: scale(1.2);
  border: 3px solid var(--c-light);
  text-decoration-color: var(--c-default);
}
.title {
  padding: 40px 0px;
  margin-top: 30vh;
  color: white;
  margin-bottom: -10vh;
}
h1 {
  color: var(--c-default);
  margin-bottom: 3vh;
  margin-top: 2vh;
 
}
@media only screen and (max-width: 820px){
  .service-row {
  gap: 5vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
}
.services-container {
  display: flex;
  flex-direction: column;
  justify-content: center;
  background: linear-gradient(52deg, rgb(40, 34, 34) 20%, rgb(54, 54, 54) 100%);
  width: 100%;
  /* height: 500px; */
}

.each-box {
  padding: 15px;
  border: 3px solid var(--c-default);
  transition: transform 0.6s;
  transform-style: preserve-3d;
  background-color: var(--c-cleangrey);
  width: 350px;
  height: 200px;
  font-weight: bold;
  border-radius: 20px;
  text-decoration-line: none; 
  transform: scale(0.8);
}
.each-box:hover {
  transform: scale(1.0);
  border: 3px solid var(--c-light);
  text-decoration-color: var(--c-default);
}
.title {
  padding: 40px 0px;
  margin-top: 15vh;
  color: white;
  margin-bottom: -20vh;
}
}
@media only screen and (max-height: 900px) and (max-width: 700px) {
    .service-row {
  gap: 10vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
}
.services-container {
  display: flex;
  flex-direction: column;
  justify-content: center;
  background: linear-gradient(52deg, rgb(40, 34, 34) 20%, rgb(54, 54, 54) 100%);
  width: 100%;
  /* height: 500px; */
}

.each-box {
  padding: 15px;
  border: 3px solid var(--c-default);
  transition: transform 0.6s;
  transform-style: preserve-3d;
  background-color: var(--c-cleangrey);
  width: 350px;
  height: 200px;
  font-weight: bold;
  border-radius: 20px;
  text-decoration-line: none; 
  transform: scale(0.8);
}
.each-box:hover {
  transform: scale(1.0);
  border: 3px solid var(--c-light);
  text-decoration-color: var(--c-default);
}
.title {
  padding: 40px 0px;
  margin-top: 60vh;
  color: white;
  margin-bottom: -20vh;
}
}
</style>
