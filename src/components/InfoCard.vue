<script setup lang="ts">


import {ref} from "vue";

defineProps(['title','info']);
const toggleInfo = ref(false);

</script>

<template>
  <div class="infoCard">
    <div class="infoRow" @click="toggleInfo = !toggleInfo">
      <div>{{title}}</div>
      <div v-if="!toggleInfo" class="plus">+</div>
      <div v-else class="plus">-</div>
    </div>
    <div v-if="toggleInfo" class="infoText">{{info}}</div>
  </div>

</template>

<style scoped>

.infoCard{
  border-bottom: 2px solid black;
}

.infoText{
  font-size: 1.2vw;
  margin-bottom: 2vw;
  width: 30%;
}

.infoRow{
  display: flex;
  justify-content: space-between;
  align-items: center;
  cursor: pointer;
  height: 6vh;
}

.plus{
  font-size: 4vw;
  font-weight: 300;
}


</style>
