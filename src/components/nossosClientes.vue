<template>
  <div class="clientes-container">
    <h1>Empresas que experimentaram a Always!</h1>
    <div class="section">
      <div class="each">
        <img class="img" src="@/assets/img/ciuffo.jpg" alt="" />
        Dr Ciuffo
      </div>
      <div class="each">
        <img class="img" src="@/assets/img/hungaros.jpg" alt="" />
        Doces Húngaros
      </div>
      <div class="each">
        <img class="img" src="@/assets/img/butterfly.jpg" alt="" />
       Butterflyfit88
      </div>
      <div class="each">
        <img class="img" src="@/assets/img/set.jpg" alt="" />
       Set Produções
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.clientes-container {
  display: flex;
  flex-direction: column;
  justify-content: center;
  height: auto;
  width: 100%;
  padding: 50px;
  background: linear-gradient(52deg, rgba(84,1,126,1) 2%, rgba(142,2,213,1) 50%, rgba(84,1,126,1) 92%);
}
.section {
  display: flex;
  flex-direction: row;
  gap: 10vh;
}
.img {
  height: 120px;
  width: 120px;
  border-radius: 60%;
  border: 2px solid white;
  margin-bottom: 4vh;
}
.each {
  display: flex;
  flex-direction: column;
  transition: transform 0.6s;
  transform-style: preserve-3d;
  color: var(--c-white-default);
  text-shadow: 2px 2px rgb(0, 0, 0, .4);
}
.each:hover{
    transform: scale(1.5)
}
h1{
    margin-bottom: 10vh;
    color: white;
}
img{
    transform: scale(1.2);
}
@media only screen and (max-height: 900px) and (max-width: 700px) {
.section{
    flex-direction: column;
}

}
</style>
