<template>

  <main>

    <div class="first-cta">
      <i class="fa-solid fa-paper-plane"></i>
      <span class="cta-text">get a free quote online now</span>
    </div>

    <div class="testimonial-cta">
      <div class="w-30">
        <span class="subtitle">headache free</span>

        <h2>Award Winning</h2>
        <h2 style="margin-bottom: 25px">Moving Company</h2>

        <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Voluptate dolores quis quasi cum repellat dolorem, reiciendis nesciunt, ratione consequuntur impedit nobis dicta hic corporis minima.</p>

        <a class="button" href="#testimonials">read our testimonials</a>
      </div>
    </div>

    <ServiceComponent />


    <div class="move-with-ease-section">

      <div class="move-with-ease-container">

        <div class="green-container">

          <span>we remove the headache from moving</span>
          <h3>Move With Ease</h3>

          <hr>

          <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Molestias nisi, illo velit dignissimos adipisci tenetur placeat consequatur voluptates aut odio!</p>

          <a style="font-size: 14px; font-weight: bold" class="button">get a free quote now</a>


        </div>

      </div>

    </div>


    <TestimonialsComponent 
    id="testimonials"/>

    <div class="last-cta-section">

      <div class="last-cta">

        <h2>Request A Free Quote</h2>

        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Natus dignissimos eius porro! Consectetur, at doloribus!</p>

        <a style="font-size: 13px; font-weight: bold;" class="button">click here</a>

      </div>

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

  span{
    &:hover{
      cursor: pointer;
      text-decoration: underline;
    }
  }
}

.testimonial-cta{
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;

  background-color: $light-grey-color;

  height: 500px;
  padding: 50px 0;

  p{
    color: $grey-color;
    margin-bottom: 20px;
    line-height: 1.6;
    
  }
}

.move-with-ease-section{
  background-image: url("../assets/images/avada-movers-movewithease-background-new.jpg");
  background-size: cover;
  background-repeat: no-repeat;
  height: 700px;  

  .move-with-ease-container{
  display: flex;
  justify-content: end;
  align-items: center;

  width: 70%;
  height: 100%;
  margin: 0 auto;

  .green-container{
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;

    text-align: center;

    width: 400px;
    padding: 25px 20px;

    background-color: $green-color;
    color: white;
    
    border: 12px solid #5AA511;

    span{
      text-transform: uppercase;
      margin-bottom: 10px;
      font-size: 10px;
      font-weight: bold;
    }

    h3{
      font-size: 30px;
      margin-bottom: 10px;

    }

    hr{
      height:1px;
      width:230px;
      color: rgba(255, 255, 255, 0.5);
      margin-bottom: 20px;
    }

    p{
      line-height: 1.6;
      font-size: 12px;
      margin-bottom: 20px;

    }
  }

}

}


.last-cta-section{

  background-image: url("../assets/images/avada-movers-request-quote-background.jpg");
  height: 500px;
  background-size: cover;
  border-bottom: 15px solid $green-color;

  .last-cta{
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  
  
    height: 100%;
    width: 30%;
    margin: 0 auto;
    text-align: center;
    padding: 50px 0;

    p{
      line-height: 1.6;
      margin: 20px 0;
      opacity: 0.7;
    }
  }
}




}

</style>