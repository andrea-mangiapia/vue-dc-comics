<template>
  <div id="app">
    <!-- HEADER -->
    <PageHeader/>

    <!-- MAIN -->
    <main>    
      <SectionContentMain/>
      <SectionBuyList/>    
    </main>

    <!-- FOOTER -->
    <PageFooter/>

  </div>
</template>

<script>
import PageHeader from './components/PageHeader.vue';
import PageFooter from './components/PageFooter.vue';
import SectionContentMain from './components/SectionContentMain.vue';
import SectionBuyList from './components/SectionBuyList.vue';

export default {
  name: 'App',
  components: {
    PageHeader,
    SectionContentMain,
    SectionBuyList,
    PageFooter
}
}
</script>

<style lang="scss">
@import "./style/common";

</style>
