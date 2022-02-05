<script setup>
defineProps({
  msg: String,
});
</script>

<template>
  <div class="hero">
    <p class="hero_image"></p>
    <!-- <img class="hero_image" src="../assets/camper_2.jpg" alt="" /> -->
    <div class="hero_text">
      <h1>Jessy Rent OÜ</h1>
      <ul class="hero_list">
        <li>item 1</li>
        <li>item 2</li>
        <li>item 3</li>
      </ul>


    </div>
  </div>
</template>


<style scoped>
.hero {
  height: 50vh;
  position: relative;
}
.hero_image {
  background-image: url("../assets/camper_temp.jpg");
  background-position: center;
  background-size: cover;
  -moz-background-size: cover;
  -webkit-background-size: cover;
  height: 100%;
  margin: 0;
  z-index: 0;
}
.hero_text {
  position: absolute;
  top: 50%;
  left: 50%;
  width: 100%;
  transform: translateY(-50%) translateX(-50%);
  z-index: 1;
  background-color: rgba(128, 128, 128, 0.385);
}
.hero_text h1{
  color: red;
  }
  .hero_list{
    display: flex;
    justify-content: center;
    padding-inline-start: 0;
  }
  .hero_list li{
    list-style: none;
    margin: 2rem 2rem;
  }
</style>