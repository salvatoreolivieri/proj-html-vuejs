<template>
  <footer>

    <div class="footer-top">

      <div class="footer-container">

        <h3>About</h3>

        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Adipisci incidunt consequuntur necessitatibus sint eum accusamus sapiente aliquam fuga a laborum.</p>

        <img src="../assets/images/avada-movers-retinalogo.png" alt="Avada Movers Logo">

      </div>



      <div class="footer-container">

        <h3>Avada Movers</h3>

        <ul>
          <li
          v-for="(item, index) in sitemap"
          :key="index"
          >
            <i class="fa-solid fa-chevron-right"></i>
            <a :class="item.url === 'Home' ? 'active' : ''" href="#">{{item.url}}</a>
          </li>
        </ul>


      </div>



      <div class="footer-container">

        <h3>Recent Posts</h3>

        <ul>
          <li
          v-for="(item, index) in blogPosts"
          :key="index"
          ><a href="#">{{item.title}}</a></li>
        </ul>


      </div>

    </div>

  <section>
    <div class="footer-bottom">
      <div>
        <span>&copy; Copyright 2012-2020 |  Avada Theme by ThemeFusion  |  All Rights Reserved  |  Powered by WordPress </span>
      </div>
      <div class="social-icon-container">
        <i class="fa-brands fa-facebook-f"></i>
        <i class="fa-brands fa-twitter"></i>
        <i class="fa-brands fa-instagram"></i>
        <i class="fa-brands fa-youtube"></i>
      </div>
    </div>
  </section>

  </footer>
</template>

<script>
export default {
  name: "FooterComponent",
  data(){
    return{
      sitemap:[
        {
          url: "Home"
        },
        {
          url: "Rates"
        },
        {
          url: "Testimonials"
        },
        {
          url: "Blog"
        },
        {
          url: "Free Quote"
        },
      ],
      blogPosts: [
        {
          title: "Heading Out to College?"
        },
        {
          title: "Moving Your Business"
        },
        {
          title: "Outstanding Quality"
        },
        {
          title: "Cost Of Moving"
        },
        {
          title: "Best Moving Tips"
        },
      ]
    }
  }
}
</script>

<style lang="scss" scoped>

@import "../assets/style/var";

footer{

  .footer-top,
  .footer-bottom{
    width: 70%;
    margin: 0 auto;

  }

  .footer-top{
    display: flex;
    height: 350px;
    padding: 40px 0;

    .footer-container{
      display: flex;
      flex-direction: column;
      width: 30%;
      margin-right: 30px;
      
    }

    h3{
      text-transform: uppercase;
      margin-bottom: 30px;
    }

    p{
      margin-bottom: 30px;
      line-height: 1.6;
    }

    img{
      width: 150px;
    }

    li{
      list-style: none;
      margin-bottom: 20px;

    }

    a{
      font-size: 14px;
      color: black;
      text-decoration: none;

    }

  }

  section{

    background-color: $green-color;

    .footer-bottom{
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;

      height: 120px;

      color: white;
    }

    .social-icon-container{
      margin-top: 20px;
    }

  }

  .fa-solid{
      font-size: 10px;
    }
 
}

</style>