<template>
  <div>
    <Jumbo />
    <TopInfoMain />
    <BrandsPartner/>
  </div>
</template>

<script>
import Jumbo from "./MainComponents/Jumbo.vue"
import TopInfoMain from "./MainComponents/TopInfoMain.vue"
import BrandsPartner from "./MainComponents/BrandsPartner.vue"

export default {
    name: 'Main',

    components: {
      Jumbo,
      TopInfoMain,
      BrandsPartner
    }
}
</script>

<style lang="scss" scoped>
@import "../assets/global.scss";

</style>