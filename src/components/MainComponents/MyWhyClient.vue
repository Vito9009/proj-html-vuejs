<template>
  <div>
      <div class="why-client-container">
          <div class="why-top-container">
              <div class="why-text">
                  <h2>We Boost Our Client's Bottom Line by Optimizing Their Growth Potential.</h2>

                  <p>Quisque aliquet, libero consequat elementum convallis, erat risus imperdiet pellentesque sem neque eget.</p>

                  <div class="my_btn-container">
                      <a href="#" class="my_header-btn">Why Work With Us</a>
                    </div>
                </div>

            </div>

            <div class="why-img">
                <img src="../../assets/img/we-boost-our-clients-600x549.jpg" alt="">
            </div>
        </div>

          <div class="why-middle-container">
              <div class="why-text-middle">
                  <div>
                      <h5>We Build Relationships</h5>

                      <p>Curabitur ac leo nunc. Vestibulum et mauris vel ante finibus maximus nec ut leo. Intreger consectetur.</p>
                  </div>

                  <div>
                      <h5>Proprietary Processes</h5>

                      <p>Curabitur ac leo nunc. Vestibulum et mauris vel ante finibus maximus nec ut leo. Intreger consectetur.</p>
                  </div>

              </div>

              <div class="why-icon-text-middle">
                  <div>
                      <img src="../../assets/img/photolight_thumbnail-400x300.jpg" alt="">

                      <div>
                          <h6>Accountability</h6>

                          <p>Curabitur ac leo nunc vestibulum</p>
                      </div>
                  </div>

                  <div>
                      <img src="../../assets/img/photolight_thumbnail-400x300.jpg" alt="">

                      <div>
                          <h6>Accountability</h6>

                          <p>Curabitur ac leo nunc vestibulum</p>
                      </div>
                  </div>

                  <div>
                      <img src="../../assets/img/photolight_thumbnail-400x300.jpg" alt="">

                      <div>
                          <h6>Accountability</h6>

                          <p>Curabitur ac leo nunc vestibulum</p>
                      </div>
                  </div>
              </div>
          </div>

          <div>
              
          </div>
    </div>
</template>

<script>

export default {
    name: 'MyWhyClient',
}
</script>

<style lang="scss" scoped>
@import "../../assets/global.scss";

.why-client-container{
    width: 60%;
    margin: 0 auto;
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 100px 0;

    .why-top-container{
        width: 50%;

        .why-text{
            padding-right: 70px;

            h2{
                font-size: 30px;
                margin-bottom: 30px;
            }

            p{
                font-size: 15px;
                margin-bottom: 30px;
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
                    font-weight: bold;
                }
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

    .why-middle-container{
        display: flex;
        justify-content: center;
    }
}
</style>