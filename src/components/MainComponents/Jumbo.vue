<template>
  <div>
    <div class="my_jumbo-container">
        <div class="my_text-jumbo">
            <h1>
                Unlock Your Online Growth Potential
            </h1>

            <p>Online marketing to secure customer retention, leads, and sales. We focus on the bigger picture</p>

            <div class="my_btn-container">
                <a href="#" class="my_jumbo-btn">Our Services <i class="fa-solid fa-arrow-right"></i></a>
            </div>
        </div>

        <div class="marketing-consultant-card">
            <MarketingConsultantExpertCard />
        </div>

        <div class="mini-box-container">
            <div class="box-1"><img src="../../assets/img/demos.png" alt=""></div>
            <div class="box-2"><img src="../../assets/img/on-sale.png" alt=""></div>
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

    .mini-box-container{
        position: absolute;
        right: 10px;
        top: 100px;

        .box-1, .box-2{
            height: 40px;
            width: 40px;
            background-color: $whiteColor;
            margin-bottom: 4px;
            border-radius: 5px;
            display: flex;
            justify-content: center;
            align-items: center;
            
            img{
                width: 80%;
            }
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
            margin: 30px 0;
        }
    }

    .my_btn-container{
        height: 100%;
        display: flex;
        align-items: center;
        
        .my_jumbo-btn{
            padding: 10px 30px;
            color: $blackColor;
            background-color: $whiteColor;
            border-radius: 5px;
            text-decoration: none;
            font-weight: bold;
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