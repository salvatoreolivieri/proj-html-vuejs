<template>

  <section class="hero-section">
    <div class="text-container">
      <span>moving without the hassle</span><br>
      <h1>we make it simple</h1>
      <span>professional service with quality and customer satisfaction</span>
    </div>
  </section>
  
</template>

<script>
export default {
  name:"HeroSection.vue"
}
</script>

<style lang="scss" scoped>

@import "../assets/style/var";

.hero-section{
  height: 730px;
  margin-top: -80px;
  background-image: url("../assets/images/avada-movers-homeherobackground-final.jpg");
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;

  text-transform: uppercase;

  .text-container {
    height: 100%;
    width: 100%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;

    h1{
      font-size: 55px;
      margin: 15px 0;
    }

    span{
      font-size: 14px;
    }
  }

}

</style>