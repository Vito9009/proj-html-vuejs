<template>
  <div>
    <Jumbo />
    <TopInfoMain />
  </div>
</template>

<script>
import Jumbo from "./MainComponents/Jumbo.vue"
import TopInfoMain from "./MainComponents/TopInfoMain.vue"

export default {
    name: 'Main',
    components: {
      Jumbo,
      TopInfoMain
    }
}
</script>

<style lang="scss" scoped>
@import "../assets/global.scss";

</style>