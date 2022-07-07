<template>
  <footer>
    <!-- Footer Top -->
    <div class="footer-main">
      <div class="container am-flex">
        <div class="col-left am-flex">
          <div class="menu-footer">
            <h3>
              Dc Comics
            </h3>
            <ul>
              <li><a href="#">Characters</a></li>
              <li><a href="#">Comics</a></li>
              <li><a href="#">Movies</a></li>
              <li><a href="#">TV</a></li>
              <li><a href="#">Games</a></li>
              <li><a href="#">Videos</a></li>
              <li><a href="#">News</a></li>
            </ul>

            <h3>
              Shop
            </h3>
            <ul>
              <li><a href="#">Shop DC</a></li>
              <li><a href="#">Shop DC Collectibles</a></li>
            </ul>
          </div>
          <div class="menu-footer">
            <h3>
              Dc
            </h3>
            <ul>
              <li><a href="#">Terms Of Use</a></li>
              <li><a href="#">Privacy policy (New)</a></li>
              <li><a href="#">Ad Choices</a></li>
              <li><a href="#">Advertising</a></li>
              <li><a href="#">Jobs</a></li>
              <li><a href="#">Subscriptions</a></li>
              <li><a href="#">Talent Workshops</a></li>
              <li><a href="#">CPSC Certificates</a></li>
              <li><a href="#">Ratings</a></li>
              <li><a href="#">Shop Help</a></li>
              <li><a href="#">Contact Us</a></li>
            </ul>
          </div>
          <div class="menu-footer">
            <h3>
              Sites
            </h3>
            <ul>
              <li><a href="#">DC</a></li>
              <li><a href="#">MAD Magazine</a></li>
              <li><a href="#">DC Kids</a></li>
              <li><a href="#">DC Universe</a></li>
              <li><a href="#">DC Power Visa</a></li>
            </ul>
          </div>
        </div>
        <div class="col-right">
          <img src="../assets/img/dc-logo-bg.png" alt="">
        </div>
      </div>          
    </div>

    <!-- Footer Bottom -->
    <div class="footer-bottom">
      <div class="container am-flex">
        <div class="left">
          <button>Sign-Up Now!</button>
        </div>
        <div class="right">
          Testo right
        </div>
      </div>
      
    </div>
               
  </footer>
</template>

<script>
export default {
  name: 'PageFooter',

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "../style/variables";
.footer-main {
  padding: 20px 0;
  background-image: url(../assets/img/footer-bg.jpg);
  color: white;
  position: relative;
  
  .col-left {
    h3 {
      margin: 10px 0;
    }
    .menu-footer {
      margin-right: 20px;
    }
    li {
      font-size: 12px;
      font-weight: 400;
      line-height: 17px;

      a {
        color: gray;
      }
    }
    
  }

  .col-right {
    position: absolute;
    top:-40px;
    right:50px;
    
    img {
        width: 350px;
    }
  }
}
.footer-bottom {
  padding: 20px 0;
  background-color: $brand_secondary_color;
  color: white;
  position: relative;
}

.am-flex {
    justify-content: space-between;
  }
</style>