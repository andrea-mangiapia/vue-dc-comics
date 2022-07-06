<template>
  <footer>
    <!-- Footer Top -->
    <div class="footer-main">
      <div class="container">
        Footer Top
      </div>          
    </div>

    <!-- Footer Bottom -->
    <div class="footer-bottom">
      <div class="container">
        Footer Bottom
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
  padding: 30px 0;
  background-color: grey;
}
.footer-bottom {
  padding: 20px 0;
  background-color: $brand_secondary_color;
  color: white;
}
</style>