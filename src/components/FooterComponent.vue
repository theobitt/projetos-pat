<template>
  <div class="footer">
    <div class="middle-footer">
      <div>
        Agência Always © 
        <a class="year">
          2020 - {{ this.anoAtual }}
        </a> 
      </div>
    </div>
    <div class="footer-content">

     <div>
       <img src="@/assets/icons/instagram.svg" alt="">
     </div>
     <div>
       <img src="@/assets/icons/whatsapp.svg" alt="">
     </div>
    </div>
  </div>
</template>

<script>
export default {
data(){
  return{
    anoAtual: new Date().getFullYear()
  }
}

}
</script>

<style scoped>
.footer{
  width: 100%;
  height: 40px;
  background-color: rgb(128, 128, 128, .35);
  display: flex;
  align-items: center;
  justify-content: flex-end;
}
.middle-footer{
  display: flex;
  position: relative;
  justify-content: center;
  /* margin-right: 80vh; */
  font-family: 'GothamBold', sans-serif;
  color: var(--c-default);
  text-shadow: 2px 2px 0px rgba(0, 0, 0, 0.4);
}

.year{
  text-shadow: 2px 2px 0px rgba(0, 0, 0, 0.4);
  color: white;
  margin-left: 5px;
}
.footer-content{
  display: flex;
  /* padding: 15px 10px 5px; */
  position: absolute;
  float: right;
  gap: 1vh;
  margin-right: 1vh;
}
img{
  width: 24px;
  height: 24px;
}

@media only screen and (max-height: 900px) and (max-width: 700px) { 
  .middle-footer{
  /* display: flex; */
  /* position: absolute; */
  /* justify-content: center; */
  /* margin-right: 25vh; */
  font-family: 'GothamBold', sans-serif;
  color: var(--c-default)
}

}
</style>