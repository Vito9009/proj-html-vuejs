<template>
  <div>
      <div class="container-info-main">
          <div class="info-container">
              <img src="../../assets/img/fss-demo-main-400x300.jpg" alt="">

              <div class="text-info-main">
                  <div class="min-head-container">
                      <img src="../../assets/img/award-d-200x191.png" alt="">
                      <h5>Business Growth</h5>
                    </div>
                  
                  <h2>Increase Brand Awareness</h2>
                  
                  <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed auctor placerat luctus. Nullam sit amet ante sed orci convallis gravida et at massa</p>
                  
                  <div class="my_btn-container">
                    <a href="#" class="my_header-btn">Get a Consultation</a>
                </div>
              </div>
          </div>

          <div class="info-container">
              <div class="text-info-main">
                  <div class="min-head-container">
                      <img src="../../assets/img/award-d-200x191.png" alt="">
                      <h5>Investors In People</h5>
                    </div>
                  
                  <h2>In-House Sales Training</h2>
                  
                  <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed auctor placerat luctus. Nullam sit amet ante sed orci convallis gravida et at massa</p>
                  
                  <div class="my_btn-container">
                    <a href="#" class="my_header-btn">Get a Consultation</a>
                </div>
              </div>

              <img src="../../assets/img/fss-demo-main-400x300.jpg" alt="">
          </div>

          <div class="info-container">
              <img src="../../assets/img/fss-demo-main-400x300.jpg" alt="">

              <div class="text-info-main">
                  <div class="min-head-container">
                      <img src="../../assets/img/award-d-200x191.png" alt="">
                      <h5>Social Media Analysis</h5>
                    </div>
                  
                  <h2>Harness Your Social Proof</h2>
                  
                  <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed auctor placerat luctus. Nullam sit amet ante sed orci convallis gravida et at massa</p>
                  
                  <div class="my_btn-container">
                    <a href="#" class="my_header-btn">Get a Consultation</a>
                </div>
              </div>
          </div>

      </div>
  </div>
</template>

<script>

export default {
    name: 'TopInfoMain'
}
</script>

<style lang="scss" scoped>
@import "../../assets/global.scss";

.container-info-main{
    width: 75%;
    margin: 100px auto;

    .info-container{
        display: flex;
        justify-content: space-around;
        align-items: center;
        margin: 100px 0;

        .text-info-main{
            width: 40%;
            padding: 60px;
            display: flex;
            flex-direction: column;

            .min-head-container{
                display: flex;
                align-items: center;
                margin-bottom: 10px;

                img{
                    height: 30px;
                    margin-right: 5px;
                }

                h5{
                    font-size: 11px;
                }
            }
            
            h2{
                font-size: 30px;
                margin-bottom: 20px;
            }

            p{
                font-size: 15px;
            }
        }

        .my_btn-container{
            height: 100%;
            display: flex;
            align-items: center;
            
            .my_header-btn{
                padding: 10px 30px;
                color: $whiteColor;
                background-color: $ecstasyColor;
                border-radius: 5px;
                text-decoration: none;
                margin-top: 20px;
                font-weight: bold;
            }
        }
    }
}
</style>