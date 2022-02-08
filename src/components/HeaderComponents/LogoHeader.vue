<template>
  <div>
      <div class="my_logo-container">
        <a href="">
            <img src="../../assets/img/avada-marketing-logo-2x-200x37.png" alt="">
        </a>
      </div>
  </div>
</template>

<script>
export default {
    name: 'LogoHeader'
}
</script>

<style lang="scss" scoped>
@import "../../assets/global.scss";

.my_logo-container{
    height: 100%;
    display: flex;
    align-items: center;

    a{
        img{
            height: 25px;
        }
    }
}

</style>