<template>
    <!-- Single Card -->
    <div class="single-card">
        <!-- Image Card -->
        <div class="img-card">
            <img src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX" alt="">
        </div>
        <!-- Title Series Card -->
        <h2 class="series-card">
            Action Comics
        </h2>
    </div>

</template>

<script>
export default {
  name: 'SingleCard',

}
</script>

<style scoped lang="scss">

.single-card {
width: calc((100% / 6) - 20px);
margin: 10px 10px 30px 10px;

    .series-card {
        margin-top: 10px;
        font-size: 14px;
    }
}

</style>