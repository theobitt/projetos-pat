<template>
  <button class="button">
    <span> {{ text }} </span>
    <img src="@/assets/icons/wpp2.svg" alt="">
  </button>
</template>

<script>
export default {
  props: {
    text: {
      type: String,
      required: true
    }
  },
    // eslint-disable-next-line
    name: "Button",
}
</script>

<style scoped>
button {
  height: 42px;
  border: none;
  background-color: var(--c-default);
  color: #fff;
  border-radius: 4px;
  transition: background 0.2s ease-in;
  display: flex;
  align-items: center;
  /* justify-content: center; */
  width: 450px;
  font-family: 'GothamBold';
  font-size: 22px;
}

button:hover {
  color: var(--c-white-default);
  background-color: var(--c-default2);
  cursor: pointer;
}

span {
  text-align: left;
  background-color: transparent;
  font-weight: bold;
  margin-left: 40px;
  text-shadow: 2px 2px 0px rgba(0,0,0,0.1);

}
img{
  position: absolute;
  margin-left: 375px;
  transform: scale(1.5);
  width: 16px;
  height: 16px;
  filter: invert(100%) sepia(100%) saturate(0%) hue-rotate(248deg) brightness(107%) contrast(102%);
}
img:hover{
  cursor: pointer;
  /* opacity: 0.7; */
}

@media only screen and (max-height: 900px) and (max-width: 700px) {
  button {
  height: 42px;
  border: none;
  background-color: var(--c-default);
  color: #fff;
  border-radius: 4px;
  transition: background 0.2s ease-in;
  display: flex;
  align-items: center;
  /* justify-content: center; */
  width: 250px;
  font-family: 'GothamBold';
  font-size: 15px;
}
span {
  text-align: left;
  background-color: transparent;
  font-weight: bold;
  margin-left: 10px;
  text-shadow: 2px 2px 0px rgba(0,0,0,0.1);

}
img{
  position: absolute;
  margin-left: 225px;
  transform: scale(0.7);
  width: 16px;
  height: 16px;
  filter: invert(100%) sepia(100%) saturate(0%) hue-rotate(248deg) brightness(107%) contrast(102%);
}
}
</style>
