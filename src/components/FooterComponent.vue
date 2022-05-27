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
          <li><a class="active" href="#">Home</a></li>
          <li><a href="#">Rates</a></li>
          <li><a href="#">Testimonials</a></li>
          <li><a href="#">Blog</a></li>
          <li><a href="#">Free Quote</a></li>
        </ul>


      </div>



      <div class="footer-container">

        <h3>Recent Posts</h3>

        <ul>
          <li><a href="#">Heading Out to College?</a></li>
          <li><a href="#">Moving Your Business</a></li>
          <li><a href="#">Outstanding Quality</a></li>
          <li><a href="#">Cost Of Moving</a></li>
          <li><a href="#">Best Moving Tips</a></li>
        </ul>


      </div>

    </div>

  <section>
    <div class="footer-bottom">
      <span>&copy; Copyright 2012-2020 | Avada Theme by ThemeFusion | All Rights Reserved | Powered by WordPress </span>
      <span style="margin-top: 15px;">social icon</span>
    </div>
  </section>

  </footer>
</template>

<script>
export default {
  name: "FooterComponent"
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

    span{}

  }

  

  
}

</style>