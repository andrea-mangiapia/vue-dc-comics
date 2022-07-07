<template>
    <!-- Single Card -->
    <div class="single-card">
        <!-- Image Card -->
        <div class="img-card">
            <img :src="cardDetails.thumb" :alt="cardDetails.series">
        </div>
        <!-- Title Series Card -->
        <h2 class="series-card">
            {{cardDetails.series}}
        </h2>
    </div>

</template>

<script>
export default {
  name: 'SingleCard',
  props: {
        cardDetails: Object
    },

}
</script>

<style scoped lang="scss">

.single-card {
width: calc((100% / 6) - 20px);
margin: 10px 10px 30px 10px;

    .img-card {

        img {
            width: 100%;
            object-fit: cover;
            object-position: top;
            aspect-ratio: 1 / 1;
        }
    }
    

    .series-card {
        margin-top: 10px;
        font-size: 14px;
    }
}

</style>