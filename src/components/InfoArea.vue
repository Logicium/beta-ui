<script setup lang="ts">

import InfoCard from "@/components/InfoCard.vue";
</script>

<template>

  <div class="infoWrap">
    <InfoCard title="01 ABOUT" info="We are a micro design studio based in Trinidad, CO. Est. 2024."/>
    <InfoCard title="02 MISSION" info="Our mission is to crete designs that inspire, both an art and a science."/>
    <InfoCard title="03 LOCATION" info="Located at 256 1st Street, Trinidad CO 81082"/>
  </div>

</template>

<style scoped>

.infoWrap{
  margin: 2vw;
  display: flex;
  flex-direction: column;
  font-size: 1.5vw;
}

</style>
