<template>
  <div class="container">
    <div class="wide-purple-container">
      <div class="items-container">
        <div class="each-item">
          <img src="@/assets/icons/coffe.svg" alt=""> 
          +12 colaboradores! 
        </div>
        <div class="each-item">
          <img src="@/assets/icons/cash.svg" alt=""> 
          +R$17.000 investidos!
        </div>
        <div class="each-item">
          <img src="@/assets/icons/celebrate.svg" alt=""> 

          +3 anos no mercado
        </div>
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
img{
  filter: invert(100%) sepia(100%) saturate(0%) hue-rotate(248deg) brightness(107%) contrast(102%);
  transform: scale(0.8);
  width: 40px;
  height: 40px;
  transition: transform 0.6s;
  transform-style: preserve-3d;
}
img:hover{
  transform: rotateY(180deg);

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
.each-item{
  display: flex;
  flex-direction: column;
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
  padding: 60px;
  width: 100%;
  height: 100%;
  display: flex;
  flex-direction: column;
  font-size: 22px;
  gap: 14vh;

}
}
</style>
