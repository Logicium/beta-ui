<script setup lang="ts">
import Navbar from "@/components/Navbar.vue";
import ImageArea from "@/components/ImageArea.vue";
import Footer from "@/components/Footer.vue";
import CtaArea from "@/components/CtaArea.vue";
import InfoArea from "@/components/InfoArea.vue";
</script>

<template>

  <div class="webapp">

    <Navbar/>

    <ImageArea/>

    <InfoArea/>

    <CtaArea/>

    <Footer/>

  </div>

</template>

<style scoped>

.webapp{
  display: flex;
  flex-direction: column;
  position: relative;
  padding-bottom: 2vw;
}

</style>
