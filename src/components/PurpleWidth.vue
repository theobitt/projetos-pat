<template>
  <div class="container">
    <div class="wide-purple-container">
      <div class="items-container">
        <div>+12 colaboradores!</div>
        <div>+R$17.000 investidos!</div>
        <div>+3 anos no mercado</div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.container {
  display: flex;
  flex-direction: column;
  width: 100%;
  height: auto;
  position: static;
}
.wide-purple-container {
  display: flex;
  flex-direction: row;
  background: linear-gradient(52deg, rgba(84,1,126,1) 2%, rgba(142,2,213,1) 50%, rgba(84,1,126,1) 92%);

  color: white;
  gap: 3vh;
  width: 100%;
  text-shadow: 2px 2px 0px rgba(0, 0, 0, 0.4);
  height: 200px;
  top: 400px;
  position: absolute;
}
.items-container {
  align-items: center;
  padding: 40px;
  width: 100%;
  height: 100%;
  display: flex;
  flex-direction: row;
  font-size: 32px;
}
@media only screen and (max-height: 653px){
  .wide-purple-container {
  display: flex;
  flex-direction: column;
  background: linear-gradient(52deg, rgba(84,1,126,1) 2%, rgba(142,2,213,1) 50%, rgba(84,1,126,1) 92%);
  color: white;
  gap: 3vh;
  width: 100%;
  text-shadow: 2px 2px 0px rgba(0, 0, 0, 0.4);
  height: 400px;
  /* top: 400px; */
  position: absolute;
}
.items-container {
  /* margin-top: 0vh; */
  align-items: center;
  padding: 40px;
  width: 100%;
  height: 100%;
  display: flex;
  flex-direction: column;
  font-size: 22px;
  gap: 14vh;

}
}
</style>
