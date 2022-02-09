<template>
  <div>
    <Jumbo />
    <TopInfoMain />
    <BrandsPartner />
    <CaseStudiesSectionMain />
  </div>
</template>

<script>
import Jumbo from "./MainComponents/Jumbo.vue"
import TopInfoMain from "./MainComponents/TopInfoMain.vue"
import BrandsPartner from "./MainComponents/BrandsPartner.vue"
import CaseStudiesSectionMain from "./MainComponents/CaseStudiesSectionMain.vue"


export default {
    name: 'Main',

    components: {
      Jumbo,
      TopInfoMain,
      BrandsPartner,
      CaseStudiesSectionMain
    }
}
</script>

<style lang="scss" scoped>
@import "../assets/global.scss";

</style>