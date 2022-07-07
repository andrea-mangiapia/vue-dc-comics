<template>
    <section class="content-main">
        <div class="container">
            <h2>
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

.content-main {
    background-color: $section_color_primary;
    color: white;
    padding: 30px 0;
    text-transform: uppercase;    
}

.cards {
    display: flex;
    flex-wrap: wrap;
}

</style>