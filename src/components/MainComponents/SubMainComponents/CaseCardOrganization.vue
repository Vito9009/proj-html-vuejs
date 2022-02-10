<template>
  <div class="my_card-container">
      <img :src="img" alt="">
      <p class="main-text">{{mainText}}</p>
      <h2>{{text}}</h2>
      <p class="sub-text">{{subText}}</p>
  </div>
</template>

<script>

export default {
    name: 'CaseCardOrganization',
    props:{
        img: String,
        mainText: String,
        text: String,
        subText: String
    }
}
</script>

<style lang="scss" scoped>
@import "../../../assets/global.scss";

.my_card-container{
    margin: 0 20px;

    img{
        width: 250px;
    }

    .main-text{
        padding-top: 20px;
        padding-bottom: 10px;
        font-size: 18px;
        border-bottom: 1px dotted $gunsmokeColor;

    }

    h2{
        font-size: 30px;
        margin-bottom: 3px;
        padding-top: 10px;
    }

    .sub-text{
        font-size: 12px;
        color: $tundoraColor;
    }
}
</style>