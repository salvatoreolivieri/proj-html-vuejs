<template>
  <div class="testimonial-card">
  
        <div class="img-container">
          <img :src="getImgUrl(testimonial.img)" alt="">
        </div>
  
        <div class="text-container">
          <h3>{{testimonial.name}}</h3>
          <p>{{testimonial.feedback}}</p>
        </div>
  
      </div>
</template>

<script>
export default {
  name: "TestimonialCardComponent",
  props:{
    testimonial : Object,
  },
  methods: {
    getImgUrl(pic){
      return require ("../assets/images/"+pic)
    }
  }
}
</script>

<style lang="scss" scoped>

@import "../assets/style/var";

.testimonial-card{
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;

      width: calc((100% / 3) - 100px);

      margin-bottom: 100px;
      margin-right: 30px;

      .img-container{
      width: 100px;

        img{
          border-radius: 50%;
          width: 100%;
        }
      }

      h3{
        color: $blue-color;
        margin: 20px 0;
      }

      p{
        line-height: 1.6;
        opacity: 0.5;
        font-style: italic;
      }

    }


</style>