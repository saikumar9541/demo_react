<template>
  <div class="container">
    <div class="valentines-card">
      <h1 class="title">Happy Valentine's Day!</h1>
      <div class="love-symbols">
        <img src="/Love_Heart_symbol.svg.png" alt="Love Symbol" class="image"/>
        <img src="/personal.jpg" alt="Your Image" class="overlay-image"/>
      </div>
      <p class="message">{{ message }}</p>
      <h1 class="heading">Love You</h1>
    </div>
  </div>
</template>

<script setup lang="ts">
  const message = ref("To my love, you mean everything to me. Happy Valentine's Day!");
</script>

<style scoped>
.container {
  animation: alternate;
  text-align: center;
  align-items: center;
}
.valentines-card {
  text-align: center;
  align-items: center;
  padding: 20px;
  height:500px;
  width: 400px;
  border: 2px solid purple;
  background-color: lightsteelblue;
}

.title {
  font-size: 24px;
  color: red;
}

.love-symbols {
  margin: 20px 0;
  position: relative;
}

.image {
  width:300px !important;
  height: auto;
}

.overlay-image {
  position: absolute;
  top: 40%;
  left: 50%;
  transform: translate(-50%, -50%);
  max-width: 80%;
  max-height: 80%;
  height:100px;
  width: 100px;
}

.message {
  font-size: 18px;
  color: #333;
}

.heading {
  color: purple;
}

/* Add animations if needed */
</style>

