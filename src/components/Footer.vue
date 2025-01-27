<script setup lang="ts">

</script>

<template>
  <div class="footerWrap">

    <div class="footerTop">
      <div>
        <div class="visit">Visit Us</div>
        <div class="address">256 1st Street, Trinidad CO 81082</div>
      </div>
      <div class="appLetter">B</div>
    </div>

    <div class="footer">
      <div>2025</div>
      <div>Beta all rights reserved</div>
    </div>

  </div>
</template>

<style scoped>


.footerWrap{
  padding: 2vw;
  display: flex;
  flex-direction: column;
  margin:0 2vw 0 2vw;
  background-color: black;
  color: #f8f4f0;
  border-radius: 30px;
  height:30vh;
}

.footerTop{
  display: flex;
  justify-content: space-between;
  align-items: end;
  height: 6vh;
  margin-top: auto;
  margin-bottom: 0.5vw;
}

.visit{
  font-size: 1.5vw;
}

.footer{
  margin-top: 0.5vw;
  display: flex;
  height: 6vh;
  justify-content: space-between;
  align-items: center;
  border-top: 2px solid #f8f4f0;
}

.appLetter{
  font-size: 2.5vw;
  line-height: 2.5vw;
  font-weight: 400;
  font-family: "Monoton", serif;
}


</style>
