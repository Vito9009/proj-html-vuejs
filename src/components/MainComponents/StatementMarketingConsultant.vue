<template>
  <div>
      <div class="why-client-container">
          <div class="my-top-container">
            <div class="why-top-container">
                <div class="why-img">
                    <img src="../../assets/img/large-testimonial-600x583.jpg" alt="">
                </div>

                <div class="why-text">
                    <p class="statement">"The team at Avada Marketing Consultant is fabulous. They helped us unlock our potential online and offline. We have experienced year on year growth due to thei progressive approach."</p>

                    <p class="name-consultant">Kate Schadler</p>

                    <p class="profession-role">Marketing Consultant - Abstract</p>
                </div>
          </div>
        </div>
    </div>
</div>
</template>

<script>

export default {
    name: 'StatementMarketingConsultant'
}
</script>

<style lang="scss" scoped>
@import "../../assets/global.scss";

.why-client-container{
    width: 60%;
    margin: 0 auto;
    padding: 100px 0;

    .my-top-container{
        display: flex;
        justify-content: center;
        align-items: center;
        .why-top-container{
            display: flex;

            .why-text{
                width: 50%;
                padding: 0 80px;
                display: flex;
                flex-direction: column;
                justify-content: center;

                .statement{
                    font-size: 18px;
                    margin-bottom: 20px;
                    font-weight: bold;
                }

                .name-consultant{
                    font-size: 12px;
                    margin-bottom: 5px;
                    font-weight: bold;
                }

                .profession-role{
                    font-size: 9px;
                    color: $tundoraColor;
                }
            }
        }

        .why-img{
            width: 50%;

            img{
                width: 100%;
                border-radius: 5px;
            }
        }
    }
}
</style>