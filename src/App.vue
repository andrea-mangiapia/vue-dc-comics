<template>
  <div id="app">
    <!-- HEADER -->
    <PageHeader/>

    <!-- MAIN -->
    <main>   
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
import SectionCard from './components/SectionCard.vue';
import SectionContentMain from './components/SectionContentMain.vue';
import SectionBuyList from './components/SectionBuyList.vue';
import PageFooter from './components/PageFooter.vue';

export default {
  name: 'App',
  components: {
    PageHeader,
    SectionCard,
    SectionContentMain,
    SectionBuyList,
    PageFooter
}
}
</script>

<style lang="scss">
@import "./style/common";

</style>
