<template>
    <section class="content-main">
        <div class="container">
            <h2 class="title-section">
                Current Series
            </h2>

            <div class="cards">
                <SingleCard v-for="element, index in cards" :key="index" :cardDetails="element" />                

            </div>

        </div>
    </section>
</template>

<script>
import CardsJson from '../assets/data/dc-comics.json';
import SingleCard from './SingleCard.vue';

export default {
    name: "SectionCard",
    components: {
        SingleCard
    },
    data() {
        return {
            cards: CardsJson
        };
    }
}
</script>

<style scoped lang="scss">
@import "../style/variables";


.section{
    position: absolute;
}
.content-main {
    background-color: $section_color_primary;
    color: white;
    text-transform: uppercase;    
}

.cards {
    display: flex;
    flex-wrap: wrap;
}

.title-section {
    background-color: $brand_main_color;
    color: white;
    display: inline-block;
    padding: 7px 20px;
    position: relative;
    top: -20px;
}

</style>