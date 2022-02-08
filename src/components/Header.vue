<template>
  <header>
    <div class="my_header-container">
      <LogoHeader />
      <LinkHeader />
      <ContactHeader />
      <ButtonHeader />
    </div>
  </header>
</template>

<script>
import LogoHeader from "./HeaderComponents/LogoHeader.vue"
import LinkHeader from "./HeaderComponents/LinkHeader.vue"
import ContactHeader from "./HeaderComponents/ContactHeader.vue"
import ButtonHeader from "./HeaderComponents/ButtonHeader.vue"

export default {
    name: 'Header',
    components: {
      LogoHeader,
      LinkHeader,
      ContactHeader,
      ButtonHeader
    }
}
</script>

<style lang="scss" scoped>
@import "../assets/global.scss";

header{
  height: 80px;
  display: flex;
  align-items: center;
  
  .my_header-container{
    width: 75%;
    margin: 0 auto;
    display: flex;
    justify-content: space-between;
  }
}
</style>