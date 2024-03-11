<template>
  <div class="content">
    <div class="image">
      <AnimatedPlaceholder width="100px" height="100px" borderRadius="50%" />
    </div>
    <div class="text">
      <AnimatedPlaceholder width="100px" height="20px" />
      <AnimatedPlaceholder width="150px" height="20px" />
    </div>
    <div class="social">
      <AnimatedPlaceholder width="30px" height="30px" borderRadius="50%" />
      <AnimatedPlaceholder width="30px" height="30px" borderRadius="50%" />
      <AnimatedPlaceholder width="30px" height="30px" borderRadius="50%" />
      <AnimatedPlaceholder width="30px" height="30px" borderRadius="50%" />
      <AnimatedPlaceholder width="30px" height="30px" borderRadius="50%" />
      <AnimatedPlaceholder width="30px" height="30px" borderRadius="50%" />
    </div>
    <div class="principal-content">
      <AnimatedPlaceholder width="500px" height="200px" />
    </div>
    <div class="more-content">
      <AnimatedPlaceholder />
      <AnimatedPlaceholder />
      <AnimatedPlaceholder />
      <AnimatedPlaceholder />
    </div>
  </div>
</template>

<script setup>
import AnimatedPlaceholder from './AnimatedPlaceholder.vue';
</script>

<style scoped>
.text {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 10px;
}

.more-content {
  display: flex;
  flex-wrap: wrap;
  align-items: center;
  gap: 10px;
}

.more-content > * {
  width: 240px;
  height: 130px;
  border-radius: 10px;
}

/* responsivo */
@media (max-width: 620px) {
  .content {
    padding: 20px 30px;
    width: 100%;
  }
  .principal-content {
    width: 100%;
  }
  .principal-content > * {
    width: 311px;
    max-width: 100%;
    height: 130px;
  }
  .more-content > * {
    width: 46%;
    height: 80px;
  }
}
</style>