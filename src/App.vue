<template>
  <div id="app">
    <!-- HEADER -->
    <PageHeader/>

    <!-- MAIN -->
    <main>
      <SectionJumbotron />  
      <SectionCard/> 
      <SectionContentMain/>
      <SectionBuyList/>    
    </main>

    <!-- FOOTER -->
    <PageFooter/>

  </div>
</template>

<script>
import PageHeader from './components/PageHeader.vue';
import SectionJumbotron from './components/SectionJumbotron.vue';
import SectionCard from './components/SectionCard.vue';
import SectionBuyList from './components/SectionBuyList.vue';
import PageFooter from './components/PageFooter.vue';

export default {
  name: 'App',
  components: {
    PageHeader,
    SectionJumbotron,
    SectionCard,
    SectionBuyList,
    PageFooter
}
}
</script>

<style lang="scss">
@import "./style/common";
main {
  margin-top: 100px;
}

</style>
