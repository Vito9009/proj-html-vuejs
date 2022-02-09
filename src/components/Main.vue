<template>
  <div>
    <Jumbo />
    <TopInfoMain />
    <BrandsPartner />
    <CaseStudiesSectionMain />

    <div class="my_bg-grey">
      <MyWhyClient />
    </div>
  </div>
</template>

<script>
import Jumbo from "./MainComponents/Jumbo.vue"
import TopInfoMain from "./MainComponents/TopInfoMain.vue"
import BrandsPartner from "./MainComponents/BrandsPartner.vue"
import CaseStudiesSectionMain from "./MainComponents/CaseStudiesSectionMain.vue"
import MyWhyClient from "./MainComponents/MyWhyClient.vue"


export default {
    name: 'Main',

    components: {
      Jumbo,
      TopInfoMain,
      BrandsPartner,
      CaseStudiesSectionMain,
      MyWhyClient
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