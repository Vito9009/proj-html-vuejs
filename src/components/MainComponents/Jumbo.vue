<template>
  <div>
    <div class="my_jumbo-container">
        <div class="my_text-jumbo">
            <h1>
                Unlock Your Online Growth Potential
            </h1>

            <p>Online marketing to secure customer retention, leads, and sales. We focus on the bigger picture</p>
        </div>

        <div class="marketing-consultant-card">
            <MarketingConsultantExpertCard />
        </div>

        <div class="test">
            <div class="box-1"></div>
            <div class="box-2"></div>
        </div>
    </div>
  </div>
</template>

<script>
import MarketingConsultantExpertCard from '../ReusableComponents/MarketingConsultantExpertCard.vue'

export default {
    name: 'Jumbo',
    components: {
        MarketingConsultantExpertCard
    }
}
</script>

<style lang="scss" scoped>
@import "../../assets/global.scss";

.my_jumbo-container{
    height: 80vh;
    background-image: url("../../assets/img/marketing-intro.jpg");
    background-position: top;
    background-size: cover;
    background-repeat: no-repeat;
    color: $whiteColor;
    display: flex;
    align-items: center;
    margin-top: 80px;

    .test{
        position: absolute;
        right: 10px;
        top: 100px;
        .box-1, .box-2{
            height: 40px;
            width: 40px;
            background-color: $whiteColor;
            margin-bottom: 4px;
            border-radius: 5px;
        }
    }

    .my_text-jumbo{
        width: 500px;
        position: absolute;
        top: 30%;
        left: 15%;

        h1{
            font-size: 50px;
        }

        p{
            font-size: 20px;
        }
    }

    .marketing-consultant-card{
        width: 300px;
        position: absolute;
        top: 30%;
        right: 21%;
    }
}

</style>