<template>
  <footer>
    <!-- Footer Main -->
    <div class="footer-main">
      <div class="container am-flex">
        <div class="col-left am-flex">
          <!-- Menu Footer -->
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
          <!-- Menu Footer -->
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
          <!-- Menu Footer -->
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
      <div class="container">
        <div class="content-footer-bottom am-flex">
          <div class="left">
            <!-- Button CTA -->
            <a href="#" class="btn-cta">
                sign-up now!
            </a>
          </div>
          <!-- Icon Social -->
          <div class="icons-social">
            <h3>
              Follow Us
            </h3>
            <ul>
              <li>
                <!-- Facebook -->
                <a href="#">
                  <img src="../assets/img/footer-facebook.png" alt="Facebook">
                </a>
              </li>

              <li>
                <!-- Twitter -->
                <a href="#">
                  <img src="../assets/img/footer-twitter.png" alt="Twitter">
                </a>
              </li>

              <li>
                <!-- Youtube -->
                <a href="#">
                  <img src="../assets/img/footer-youtube.png" alt="Youtube">
                </a>
              </li>

              <li>
                <!-- Pinterest -->
                <a href="#">
                  <img src="../assets/img/footer-pinterest.png" alt="Pinterest">
                </a>
              </li>

              <li>
                <!-- Periscope -->
                <a href="#">
                  <img src="../assets/img/footer-periscope.png" alt="Periscope">
                </a>
              </li>
            </ul>
          </div>

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
.am-flex {
    justify-content: space-between;
}
.footer-main {
  padding: 20px 0;
  background-image: url(../assets/img/footer-bg.jpg);
  color: white;
  position: relative;
  
  .col-left {
    h3 {
      margin: 10px 0;
      text-transform: uppercase;
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

.content-footer-bottom {
  align-items: center;
}
.footer-bottom {
  padding: 20px 0;
  background-color: $brand_secondary_color;
  color: white;
  position: relative;
  text-transform: uppercase;

  .btn-cta {
    color: white;
    border: 2px solid $brand_main_color;
    text-decoration: none;
    padding: 10px 20px;
  }

}

.icons-social {
  display: flex;
  align-items: center;

  h3 {
    color: $brand_main_color;
  }

  .follow-us {
    text-transform: uppercase;
    color: $brand_secondary_color;
    font-size: 18px;
    font-weight: bold;
    padding-right: 20px;
  }

  ul {
    display: flex;
    
    li {
      margin: 0 10px;
    }
  }
}
</style>