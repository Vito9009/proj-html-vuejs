<template>
  <header>
    <div class="my_header-container">
      <MyLogoHeader />
      <LinkHeader />
      <ContactHeader />
      <ButtonHeader />
    </div>
  </header>
</template>

<script>
import MyLogoHeader from "./HeaderComponents/MyLogoHeader.vue"
import LinkHeader from "./HeaderComponents/LinkHeader.vue"
import ContactHeader from "./HeaderComponents/ContactHeader.vue"
import ButtonHeader from "./HeaderComponents/ButtonHeader.vue"

export default {
    name: 'Header',
    components: {
      MyLogoHeader,
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
  background-color: $whiteColor;
  display: flex;
  align-items: center;
  position: fixed;
  top: 0;
  right: 0;
  left: 0;
  z-index: 1;
  
  .my_header-container{
    width: 75%;
    margin: 0 auto;
    display: flex;
    justify-content: space-between;
  }
}
</style>