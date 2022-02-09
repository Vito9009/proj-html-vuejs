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
        margin: 20px 0;
        font-size: 18px;
    }

    h2{
        font-size: 30px;
        margin-bottom: 3px;
    }

    .sub-text{
        font-size: 12px;
        color: $tundoraColor;
    }
}
</style>