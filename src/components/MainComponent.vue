<template>

  <main>

    <div class="first-cta">
      <i class="fa-solid fa-paper-plane"></i>
      <span class="cta-text">get a free quote online now</span>
    </div>

    <div class="testimonial-cta">
      <div class="w-50">
        <span class="subtitle">headache free</span>

        <h2>Award Winning</h2>
        <h2 style="margin-bottom: 25px">Moving Company</h2>

        <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Voluptate dolores quis quasi cum repellat dolorem, reiciendis nesciunt, ratione consequuntur impedit nobis dicta hic corporis minima.</p>

        <a class="button" href="#testimonials">read our testimonials</a>
      </div>
    </div>

    <ServiceComponent />

    <div class="container">
      ciao
    </div>

    <TestimonialsComponent />

    <div class="container">
      ciao
    </div>

  </main>
  
</template>

<script>
import TestimonialsComponent from './TestimonialsComponent.vue';
import ServiceComponent from './ServiceComponent.vue';
export default {
    name: "MainComponent",
    components: { TestimonialsComponent, ServiceComponent }
}
</script>

<style lang="scss" scoped>

@import "../assets/style/var";

main{

.first-cta{
  display: flex;
  justify-content: center;
  align-items: center;

  height: 100px;

  color: white;
  background-color: $blue-color;

  .cta-text{
    font-size: 14px;
    text-transform: uppercase;
  }
}

.testimonial-cta{
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;

  height: 500px;
  padding: 50px 0;

  p{
    color: $grey-color;
    margin-bottom: 20px;
    line-height: 1.6;
    
  }
}





}

</style>