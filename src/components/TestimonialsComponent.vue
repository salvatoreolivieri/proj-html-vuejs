<template>

<section class="testimonials-section">

  <div class="container">

    <div>
      <span class="subtitle">happy customers</span>
      <h2 style="margin: 10px 0">Testimonials</h2>
    </div>

    <div class="testimonial-card-container">

      <TestimonialCardComponent
      v-for="(item, index) in testimonials"
      :key="index"
      :testimonial=item
      />

    </div>

    <div>
      <a style="font-size:14px; font-weight: bold;" class="button">read more testimonials</a>
    </div>

  </div>
</section>
  
</template>

<script>
import TestimonialCardComponent from './TestimonialCardComponent.vue';
export default {
    name: "TestimonialsComponent",
    components: { TestimonialCardComponent },

    data(){
      return{
        testimonials : [

          {
            img: "avada-movers-johndoe-final.jpg",
            name: "John Doe",
            feedback: "Lorem ipsum dolor sit amet, consectetur adipisicing elit. Corporis culpa neque at consectetur, voluptas ex illo ea error nisi saepe assumenda nobis dolor hic aut maxime maiores magnam. Iste, ut."
          },

          {
            img: "avada-movers-janedoe-final.jpg",
            name: "Jane Doe",
            feedback: "Lorem ipsum dolor sit amet, consectetur adipisicing elit. Corporis culpa neque at consectetur, voluptas ex illo ea error nisi saepe assumenda nobis dolor hic aut maxime maiores magnam. Iste, ut."
          },

          {
            img: "avada-movers-johnsmith-final.jpg",
            name: "John Smith",
            feedback: "Lorem ipsum dolor sit amet, consectetur adipisicing elit. Corporis culpa neque at consectetur, voluptas ex illo ea error nisi saepe assumenda nobis dolor hic aut maxime maiores magnam. Iste, ut."
          },

        ]
      }
    }
}
</script>

<style lang="scss" scoped>

@import "../assets/style/var";

.testimonials-section{
  background-image: url("../assets/images/avada-movers-testimonial-background.jpg");
  background-size: cover;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  margin-bottom: 50px;

  .testimonial-card-container{
    display: flex;
    justify-content: center;
    margin-top: 30px;

  }


}

</style>