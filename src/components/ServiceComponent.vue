<template>
  <div class="container">
    <span class="subtitle">we are professional</span>
    <h2>Full-Service Solution</h2>

    <div class="card-container">

      <CardComponent
      v-for="(item, index) in services" :key="`service${index}`"
      :service="item"
      /> 

    </div>

  </div>
</template>

<script>
import CardComponent from './CardComponent.vue';
export default {
    name: "ServiceComponent",
    components: { CardComponent },
    data(){
      return{
        services: [

          {
            img: "avada-movers-serviceonephoto-final.jpg" ,
            title: "Two Man Teams",
            description: "Lorem ipsum dolor sit amet, consectetur adipisicing elit. Distinctio fuga quisquam neque voluptatibus, officia assumenda perferendis modi!",
          },

          {
            img: "avada-movers-servicetwophoto-final.jpg" ,
            title: "We Do All The Lifting",
            description: "Lorem ipsum dolor sit amet, consectetur adipisicing elit. Distinctio fuga quisquam neque voluptatibus, officia assumenda perferendis modi!",
          },

          {
            img: "avada-movers-servicethreephoto-final.jpg" ,
            title: "Coast To Coast",
            description: "Lorem ipsum dolor sit amet, consectetur adipisicing elit. Distinctio fuga quisquam neque voluptatibus, officia assumenda perferendis modi!",
          },

        ]
      }
    }
}
</script>

<style lang="scss" scoped>

@import "../assets/style/var";


.card-container{

  display: flex;
  justify-content: center;

  margin-top: 30px;
}



</style>