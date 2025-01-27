<script setup lang="ts">

import MenuButton from "../components/MenuButton.vue";

</script>

<template>
  <div class="navbar">
    <div class="appTitle">BETA</div>
    <MenuButton/>
  </div>
</template>

<style scoped>

.navbar{
  display: flex;
  position: fixed;
  background-color: #f8f4f0;;
  width: 100%;
  justify-content: space-between;
  border-bottom: 2px solid black;
  align-items: center;
  height: 6vh;
  z-index: 5;
}

.appTitle{
  font-size: 2.5vw;
  font-weight: 500;
  font-family: "Monoton", serif;
  margin-left: 2vw;
  cursor: pointer;
}

</style>
