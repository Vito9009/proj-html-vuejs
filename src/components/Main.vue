<template>
  <div>
    <Jumbo />
  </div>
</template>

<script>
import Jumbo from "./MainComponents/Jumbo.vue"

export default {
    name: 'Main',
    components: {
      Jumbo
    }
}
</script>

<style lang="scss" scoped>
@import "../assets/global.scss";

</style>