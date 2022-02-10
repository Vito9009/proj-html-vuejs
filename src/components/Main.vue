<template>
  <div>
    <Jumbo />
    <TopInfoMain />
    <BrandsPartner />
    <CaseStudiesSectionMain />

    <div class="my_bg-grey">
      <MyWhyClient />
    </div>

    <StatementMarketingConsultant />

    <div class="my_bg-grey">
      <MarketingResources />
    </div>
  </div>
</template>

<script>
import Jumbo from "./MainComponents/Jumbo.vue"
import TopInfoMain from "./MainComponents/TopInfoMain.vue"
import BrandsPartner from "./MainComponents/BrandsPartner.vue"
import CaseStudiesSectionMain from "./MainComponents/CaseStudiesSectionMain.vue"
import MyWhyClient from "./MainComponents/MyWhyClient.vue"
import StatementMarketingConsultant from "./MainComponents/StatementMarketingConsultant.vue"
import MarketingResources from "./MainComponents/MarketingResources.vue"

export default {
    name: 'Main',

    components: {
      Jumbo,
      TopInfoMain,
      BrandsPartner,
      CaseStudiesSectionMain,
      MyWhyClient,
      StatementMarketingConsultant,
      MarketingResources
    }
}
</script>

<style lang="scss" scoped>
@import "../assets/global.scss";

.my_bg-grey{
  background-color: $graynurseColor;
  margin-top: 50px;
}
</style>