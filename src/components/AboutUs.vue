<template>
  <div class="about-us-container">
    <h1>Equipe <a style="color: var(--c-light) !important"> Always! </a></h1>
    <div class="photo-container">
      <div class="each-photo">
        <div class="img1" alt="" @click="whatsAppTheo()"></div>
        <h2>Theo Bittencourt</h2>
        <h4>Sócio, Gestor de tráfego e Desenvolvedor.</h4>
      </div>
      <div class="each-photo">
        <div class="img2" alt="" @click="whatsAppRilson()"></div>
        <h2>Bernardo Micati</h2>
        <h4>Sócio, Social Media e Designer.</h4>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  setup() {
    function whatsAppTheo() {
      window.open("https://api.whatsapp.com/send?phone=5521967543780");
    }
    function whatsAppRilson() {
      window.open("https://api.whatsapp.com/send?phone=5521999431819");
    }
    return {
      whatsAppTheo,
      whatsAppRilson,
    };
  },
};
</script>

<style scoped>
.about-us-container {
  display: flex;
  flex-direction: column;
  width: 100%;
  height: 500px;
  align-items: center;
  justify-content: center;
  background: linear-gradient(52deg, rgb(40, 34, 34) 20%, rgb(54, 54, 54) 100%);
  color: white;
  margin-top: 200px;
  padding: 40px;
}
.photo-container {
  display: flex;
  flex-direction: row;
  width: 100%;
  padding: 40px;
  gap: -10vh;
}
.each-photo {
  display: flex;
  flex-direction: column;
  width: 50%;
}
.img1 {
  border-radius: 60%;
  border: 10px solid var(--c-default);
  width: 250px;
  height: 250px;
  /* transform: scale(1.2); */
  background-image: url("@/assets/img/theo.png");
  background-position-x: -10px;
  background-repeat: no-repeat;
  background-size: 110%;
}
.img1:hover {
  transform: scale(1.1);
  transition: 0.7s ease-in;
  cursor: pointer;
}
.img2:hover {
  transform: scale(1.1);
  transition: 0.7s ease-in;
  cursor: pointer;
}
.img2 {
  border-radius: 60%;
  border: 10px solid var(--c-default);
  width: 250px;
  height: 250px;
  /* transform: scale(1.2); */
  background-image: url("@/assets/img/rilsete.png");
  background-position-x: -10px;
  background-repeat: no-repeat;
  background-size: 110%;
}
h1 {
  margin-top: 5vh;
}
h2 {
  font-size: 30px;
  margin-top: 2vh;
}
h4 {
  font-size: 16px;
}

@media only screen and (max-height: 900px) {
  .about-us-container {
    display: flex;
    flex-direction: column;
    width: 100%;
    height: 1300px;
    align-items: center;
    justify-content: center;
    background: linear-gradient(
      52deg,
      rgb(40, 34, 34) 20%,
      rgb(54, 54, 54) 100%
    );
    color: white;
    margin-top: 200px;
    padding: 40px;
  }
  .photo-container {
    display: flex;
    flex-direction: column;
    width: 100%;
    padding: 40px;
    justify-content: center;
    align-items: center;
    margin-right: 12vh;
  }
  .img1 {
    border-radius: 60%;
    border: 10px solid var(--c-default);
    width: 200px;
    height: 200px;
    transform: scale(0.7);
    background-image: url("@/assets/img/theo.png");
    background-position-x: -10px;
    background-repeat: no-repeat;
    background-size: 110%;
  }
  .img1:hover {
    transform: scale(0.9);
    transition: 0.7s ease-in;
    cursor: pointer;
  }
  .img2:hover {
    transform: scale(0.9);
    transition: 0.7s ease-in;
    cursor: pointer;
  }
  .img2 {
    border-radius: 60%;
    border: 10px solid var(--c-default);
    width: 200px;
    height: 200px;
    transform: scale(0.7);
    background-image: url("@/assets/img/rilsete.png");
    background-position-x: -10px;
    background-repeat: no-repeat;
    background-size: 110%;
  }
  h1 {
    margin-top: 5vh;
    float: right;
  }
  h2 {
    margin-top: 0vh;
    font-size: 15px;
    width: 100%;
  }
  h4 {
    font-size: 12px;
    margin-top: 2vh;
  }
  .each-photo {
    display: flex;
    flex-direction: column;
    width: 100%;
    align-items: center;
  }
}
@media screen and (max-height: 653px) {
    
    
}
</style>
