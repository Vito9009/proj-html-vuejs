<template>
  <div>
    <div class="my_jumbo-container">
        <div class="my_text-jumbo">
            <h1>
                Unlock Your Online Growth Potential
            </h1>

            <p>Online marketing to secure customer retention, leads, and sales. We focus on the bigger picture</p>
        </div>

        <div class="my_form-jumbo">
            <div class="consultant-expert-info">
                <img src="../../assets/img/marketing-consultant-expert.jpg" alt="">
                <h4>Richard Madsen</h4>
                <p class="grey">Marketing Consultant Expert</p>
                <span class="orange"><i class="fa-solid fa-phone"></i> (555) 802-1234</span>
            </div>

            <form action="">
                <input type="text" placeholder="Your Name*">
                <input type="text" placeholder="Your Email*">
                <input type="text" placeholder="Your Phone Number*">

                <div class="my_btn-container">
                    <a href="#" class="my_form-btn">Get a Callback</a>
                </div>
            </form>   
            
            <span class="grey">By submit my data I agree to be contacted</span>
        </div>
    </div>
  </div>
</template>

<script>
export default {
    name: 'Jumbo'
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

    .my_form-jumbo{
        width: 21%;
        height: 65%;
        background-color: $whiteColor;
        border-radius: 20px;
        display: flex;
        justify-content: space-around;
        align-items: center;
        flex-direction: column;
        color: $blackColor;
        position: absolute;
        top: 30%;
        right: 21%;

        .consultant-expert-info{
            width: 100%;
            height: 120px;
            display: flex;
            justify-content: space-around;
            align-items: center;
            flex-direction: column;
            
            img{
                height: 60px;
                border-radius: 50%;
            }
        }

        form{
            width: 90%;
            display: flex;
            flex-direction: column;

            input{
                margin-bottom: 10px;
                padding: 15px 5px;
                border-radius: 5px;
                border: 1px solid rgba(66, 66, 66, 0.3);
                outline: none;
            }

            .my_btn-container{
                    height: 100%;
                    width: 100%;
                    display: flex;
                    justify-content: center;
                    align-items: center;

                .my_form-btn{
                    width: 100%;
                    padding: 10px 0;
                    text-align: center;
                    color: $whiteColor;
                    background-color: $ecstasyColor;
                    border-radius: 5px;
                    text-decoration: none;
                }
            }
        }
    }
}

</style>