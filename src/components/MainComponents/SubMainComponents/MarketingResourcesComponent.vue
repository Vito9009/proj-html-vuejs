<template>
  <div class="my_card-resources-container">
      <img :src="img" alt="">
      <p class="text">{{text}}</p>
  </div>
</template>

<script>

export default {
    name: 'MarketingResourcesComponent',
    props:{
        img: String,
        text: String
    }
}
</script>

<style lang="scss" scoped>
@import "../../../assets/global.scss";

.my_card-resources-container{
    margin: 0 20px;

    img{
        width: 250px;
    }

    .text{
        padding-top: 20px;
        padding-bottom: 10px;
        font-size: 19px;
    }
}
</style>