<template>
  <div class="card">
  
        <div class="img-container">
          <img :src="getImgUrl(service.img)" alt="">
        </div>

        <div class="text-container">
          <h3>{{service.title}}</h3>
          <p>{{service.description}}</p>
          <a style="font-size: 12px" class="button">read more</a>
        </div>
  
  </div>
</template>

<script>
export default {
  name: "CardComponent",
  props:{
    service: Object
  },

  methods:{
    getImgUrl(pic){
      return require('../assets/images/'+pic)
    }
  }
}
</script>

<style lang="scss" scoped>

@import "../assets/style/var";

.img-container{
  width: 100%;
  margin-bottom: 10px;
  
  img{
    width: 100%;
  }
}

.text-container{
  text-align: center;
  background-color: white;
  padding: 30px 20px;

  h3{
    color: $blue-color;
  } 

  p{
    line-height: 1.6;
    margin-top: 15px;
    margin-bottom: 20px;
    font-size: 12px;
  }
}

</style>