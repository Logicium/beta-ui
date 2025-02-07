<script setup lang="ts">
import { ref } from 'vue';

const images = ['arch1.jpg', 'arch2.jpg', 'arch3.jpg'];
let imageIndex = 0;
const bigImage = ref(images[imageIndex]);

setInterval(() => {
  imageIndex = (imageIndex + 1) % images.length;
  bigImage.value = images[imageIndex];
}, 2000);
</script>

<template>
  <div class="imgWrap">

    <div class="imgTitle">BETA STUDIO</div>

    <div class="imgRow">
      <div class="imgSmall"/>
      <div class="imgBig" :style="{'background-image': `url('../../assets/${bigImage}')`}"/>
      <div class="imgSmall img2"/>
    </div>

  </div>
</template>

<style scoped>



.imgRow{
  display: flex;
  width: 80%;
  justify-content: space-evenly;
  align-items: center;
  position: absolute;
  top: 50%;
  transform: translateY(-50%);
}

.imgWrap{
  display: flex;
  flex-direction: column;
  align-items: center;
  position: relative;
  margin-top: 6vh;
  height: 70vh;
}

.imgTitle{
  position: absolute;
  text-align: center;
  font-size: 12vh;
  line-height: 12vh;
  letter-spacing: 3vw;
  font-weight: 500;
  font-family: "Monoton", serif;
  z-index: 1;
  top: 50%;
  transform: translateY(-50%);
}

.imgSmall{
  width: 15vw;
  height: 20vw;
  background-color: antiquewhite;
  background-image: url("../../assets/arch1.jpg");
  background-size: cover;
  //filter: grayscale(1);
  background-position: 100% 100%;
}

.imgBig{
  width: 25vw;
  height: 35vw;
  background-color: antiquewhite;
  //filter: grayscale(1);
  background-size: cover;
  background-position: 100% 100%;
}

.img2{
  background-image: url("../../assets/arch3.jpg");
}
</style>
