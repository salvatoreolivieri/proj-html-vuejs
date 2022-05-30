<template>
  <header>

    <section>
      <div class="header-top">

        <!-- contenitore di sinistra -->
        <div>
          <i class="fa-solid fa-phone-flip"></i>
          <span>Call us for Free Quote: 1.800.555.6789</span>
        </div>

        <!-- contenitore destra -->
        <div>
          <i class="fa-brands fa-facebook-f"></i>
          <i class="fa-brands fa-twitter"></i>
          <i class="fa-brands fa-instagram"></i>
          <i class="fa-brands fa-youtube"></i>
        </div>

      </div>
    </section>



    <div class="header-bottom">

      <div style="height:100%">
        <img style="height:100%" src="../assets/images/avada-movers-retinalogo.png" alt="Avada Movers Logo">
      </div>

      <nav>
        <ul>
          <li
          v-for="(item,index) in navItem"
          :key="index"
          >
            <a :class="item === 'Home' ? 'active' : ''" href="#">{{item}}</a>
          </li>

          <li><a class="button" href="#">free quote</a></li>
        </ul>
      </nav>

    </div>

  </header>
</template>

<script>
export default {
  name: "HeaderComponent",
  data(){
    return{
      navItem:[
        "Home",
        "Rates",
        "Testimonials",
        "FAQ",
        "Blog",
        "Contact",
      ]
    }
  }
}
</script>

<style lang="scss" scoped>

@import "../assets/style/var";

header{

  section{
    background-color: $green-color;
    color: white;
  }

  .header-top,
  .header-bottom{
    display: flex;
    justify-content: space-between;
    align-items: center;

    width: 70%;
    margin: 0 auto;

  }

  .header-top{
    height: 40px;
  }

  .header-bottom{
    height: 80px;
    padding: 10px 0;
    background-color: transparent;

    ul{
      display: flex;
    }

    li{
      list-style: none;
    }
    
    a{
      color: black;
      text-decoration: none;
      font-weight: bold;
      margin-right: 35px;

    }

  }

  
}

</style>