<template>
  <div class="wpp-container">
    <img src="@/assets/icons/wppclick.svg" alt="" @click="whatsAppTheo()">
  </div>
</template>

<script>
export default {
setup(){
    function whatsAppTheo() {
      window.open("https://api.whatsapp.com/send?phone=5521967543780");
    }
    return{
        whatsAppTheo
    }
}
}
</script>

<style scoped>
.wpp-container{
    display: flex;
    flex-direction: column;
    height: 64px;
    width: 64px;
    justify-content: right;
    position: fixed;
    float: right;
}
img {
    width: 64px;
    height: 64px;
    transform: scale(4.0);
    position: absolute;
    z-index: 3;
}
</style>