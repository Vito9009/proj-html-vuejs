<template>
  <div>
      <div class="main-brand-container">
          <div class="text-brand-container">
          <h2>Some Brands We Work With</h2>

          <p>Quisque aliquet, libero consequat elementum convallis.</p>
          </div>

          <div class="brand-container">
              <div v-for="(brand, index) in partners"
              :key="index">
                  <img class="brand-img" :src="brand.image" alt="">
              </div>
          </div>

          <div class="contact-brand-container">
                    <img src="../../assets/img/marketing-expert-cta.png" alt="">
                    <div class="consultant-info">
                        <h5>Sandy Reiff</h5>
                        <p class="grey">Marketing Consultant Expert</p>
                    </div>

                    <h5>Drive Leads and Sales with Avada</h5>

                    <span class="tel-number orange"><i class="fa-solid fa-phone"></i> (555) 802-1234</span>

  
          </div>
      </div>
  </div>
</template>

<script>

export default {
    name: 'BrandsPartner',
    data(){
      return{
        partners: [
          {
            image: require('../../assets/img/abstract.png')
          },
          {
            image: require('../../assets/img/cglobal.png')
          },
          {
            image: require('../../assets/img/next.png')
          },
          {
            image: require('../../assets/img/hemisferio.png')
          },
          {
            image: require('../../assets/img/spaces.png')
          },
          {
            image: require('../../assets/img/digitalbox.png')
          },
        ]
      }
    },
}
</script>

<style lang="scss" scoped>
@import "../../assets/global.scss";

.main-brand-container{
    width: 75%;
    margin: 0 auto;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;

    .text-brand-container{
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        margin-bottom: 25px;

        h2{
            font-size: 30px;
            margin-bottom: 10px;
        }

        p{
            font-size: 12px;
        }
    }

    .brand-container{
        display: flex;
        justify-content: center;
        
        .brand-img{
            height: 30px;
            margin: 0 30px;
        }
    }

    .contact-brand-container{
        background-color: $whiteColor;
        width: 80%;
        height: 60px;
        display: flex;
        justify-content: flex-start;
        align-items: center;
        border-radius: 5px;
        box-shadow: 0 3px 5px rgba(0, 0, 0, 0.4);
        position: relative;
        margin: 100px 0;

        img{
            height: 40px;
            border-radius: 50%;
            margin: 0 15px;
        }

        .consultant-info{
            margin-right: 40px;

            h5{
                font-size: 12px;
            }

            p{
                font-size: 10px;
            }
        }

        h5{
            font-weight: bold;
            font-size: 13px;
        }

        .tel-number{
            position: absolute;
            right: 0;
            width: 150px;
            padding: 10px 0;
            text-align: center;
            color: $ecstasyColor;
            background-color: rgba(247, 98, 16, 0.2);
            border-radius: 5px;
            margin-right: 20px;
        }
    }
}
</style>