<template>
  <div class="home-container">
    <FirstSection/>
    <PurpleWidth/>
      <about-us></about-us>
  </div>
</template>

<script>
import FirstSection from '@/components/HomeView.vue'
import PurpleWidth from '@/components/PurpleWidth.vue'
import AboutUs from '@/components/AboutUs.vue'

export default {
  // eslint-disable-next-line
  name: "Home",

  components:{
    FirstSection,
    PurpleWidth,
    AboutUs
  }
}
</script>
<style scoped>

.home-container {
  display: flex;
  flex-direction: column;
  justify-content: center;
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