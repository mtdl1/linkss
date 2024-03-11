<template>
  <div class="content">
    <div class="image">
      <img src="../assets/profile.png" alt="" />
    </div>
    <div class="text">
      <h1>Mateus Dubovicky</h1>
      <p>Frontend Developer</p>
    </div>
    <div class="social">
      <a href="https://www.instagram.com/frontdubovicky/" target="_blank">
        <ph-instagram-logo :size="32" />
      </a>
      <a href="https://twitter.com/elonmusk" target="_blank">
        <ph-twitter-logo :size="32" />
      </a>
      <a href="https://www.linkedin.com/in/mateus-dubovicky/" target="_blank">
        <ph-linkedin-logo :size="32" />
      </a>
      <a href="https://www.youtube.com/channel/UCs0w4Ynnlu6QtZ0hak2YVUA" target="_blank">
        <ph-youtube-logo :size="32" />
      </a>
      <a href="https://wa.me/5519998185588?text=Eu+quero+%F0%9F%9A%80" target="_blank">
        <ph-whatsapp-logo :size="32" />
      </a>
      <a href="mailto:mateusdubovicky@hotmail.com" target="_blank">
        <ph-envelope :size="32" />
      </a>
    </div>
    <div class="principal-content">
      <img src="https://fakeimg.pl/540x230/f1f1f1/212529/?retina=1&text=Principal%20Conte%C3%BAdo%20%F0%9F%9A%80" alt="">
    </div>
    <div class="more-content">
      <img src="https://fakeimg.pl/240x130/f1f1f1/212529/?retina=1&text=Outros%20%F0%9F%98%B6%E2%80%8D%F0%9F%8C%AB%EF%B8%8F" alt="">
      <img src="https://fakeimg.pl/240x130/f1f1f1/212529/?retina=1&text=Outros%20%F0%9F%98%B6%E2%80%8D%F0%9F%8C%AB%EF%B8%8F" alt="">
      <img src="https://fakeimg.pl/240x130/f1f1f1/212529/?retina=1&text=Outros%20%F0%9F%98%B6%E2%80%8D%F0%9F%8C%AB%EF%B8%8F" alt="">
      <img src="https://fakeimg.pl/240x130/f1f1f1/212529/?retina=1&text=Outros%20%F0%9F%98%B6%E2%80%8D%F0%9F%8C%AB%EF%B8%8F" alt="">
    </div>
  </div>
</template>

<script setup>
await new Promise((res) => setTimeout(res, 2000));
</script>

<style>
.content {
  padding: 40px 60px;
  background-color: #fff;
  box-shadow: 0 4px 6px -1px rgb(0 0 0 / 0.1),
    0 2px 4px -2px rgb(0 0 0 / 0.1);
  border-radius: 10px;
  display: flex;
  flex-direction: column;
  align-items: center;
}

.content .image {
  text-align: center;
}

.image img{
  height: 100px;
  border-radius: 50%;
}

.content .text {
  text-align: center;
  margin-top: 20px;
}

.content .text h1 {
  font-size: 24px;
  margin-bottom: 10px;
}

.content .text p {
  font-size: 18px;
  color: #666;
}

.content .social {
  margin-top: 20px;
  display: flex;
  gap: 10px;
}

.content .social a > * {
  cursor: pointer;
  background-color: #00be83;
  border-radius: 50%;
  padding: 5px;
  color: #f1f1f1;
}

.content .principal-content {
  margin-top: 40px;
  width: 100%;
  border-radius: 10px;
}

.content .principal-content img {
  width: 100%;
  border-radius: 10px;
  object-fit: cover;
  height: 200px;
  object-position: center;
}

.content .more-content {
  margin-top: 20px;
  display: flex;
  justify-content: space-between;
  flex-wrap: wrap;
  gap: 20px;
}

.content .more-content img {
  border-radius: 10px;
  width: 48%;
}

/* responsivo */
@media (max-width: 768px) {
  .content {
    padding: 20px 30px;
  }
  .content .text h1 {
    font-size: 20px;
  }
  .content .text p {
    font-size: 16px;
  }
  .content .social {
    margin-top: 10px;
  }
  .content .principal-content img {
    height: unset;
  }
  .content .more-content {
    gap: 5px;
    width: 100%;
  }
  .content .more-content img {
    width: 48%;
  }
}

</style>