<template>
  <div>
      <div class="why-client-container">
          <div class="my-top-container">
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
                  <div class="sub-icon-text-container">
                      <img src="../../assets/img/photolight_thumbnail-400x300.jpg" alt="">

                      <div>
                          <h6>Accountability</h6>

                          <p>Curabitur ac leo nunc vestibulum</p>
                      </div>
                  </div>

                  <div class="sub-icon-text-container">
                      <img src="../../assets/img/photolight_thumbnail-400x300.jpg" alt="">

                      <div>
                          <h6>Transparency</h6>

                          <p>Curabitur ac leo nunc vestibulum</p>
                      </div>
                  </div>

                  <div class="sub-icon-text-container">
                      <img src="../../assets/img/photolight_thumbnail-400x300.jpg" alt="">

                      <div>
                          <h6>Investment</h6>

                          <p>Curabitur ac leo nunc vestibulum</p>
                      </div>
                  </div>
              </div>
          </div>

          <div class="awards">
              <h5>Awards</h5>

              <div class="awards-container">
                <div class="my_awards-container">
                    <img class="hue-rotate-icon-1" src="../../assets/img/award-a-200x191.png" alt="">
                    <p class="text">Winner Seo Master MAGT Smart Start Award 2017</p>
                </div>

                <div class="my_awards-container">
                    <img src="../../assets/img/award-b-200x191.png" alt="">
                    <p class="text">Top Social Media Agencies Next Partner 2018</p>
                </div>

                <div class="my_awards-container">
                    <img class="hue-rotate-icon-3" src="../../assets/img/award-c-200x191.png" alt="">
                    <p class="text">10 Fastest Growing Abstract Solution Providers 2019</p>
                </div>

                <div class="my_awards-container">
                    <img class="hue-rotate-icon-4" src="../../assets/img/award-d-200x191.png" alt="">
                    <p class="text">National Excellence Agencie Award Winner 2020</p>
                </div>
              </div>
              <div>

              </div>

          </div>

        </div>
    </div>
</template>

<script>

export default {
    name: 'MyWhyClient'
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
    flex-direction: column;

    .my-top-container{
        display: flex;
        justify-content: center;
        align-items: center;
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
    }

    .why-middle-container{
        display: flex;
        justify-content: center;
        align-items: center;
        padding: 50px 0;

        .why-text-middle{
            width: 50%;
            padding-right: 70px;

            div{
                margin-bottom: 40px;
                h5{
                    font-size: 15px;
                    margin-bottom: 10px;
                }

                p{
                font-size: 11px;
                color: $tundoraColor;
                }
            }
        }

        .why-icon-text-middle{
            width: 50%;
            padding-right: 70px;

            .sub-icon-text-container{
                display: flex;
                justify-content: center;
                align-items: center;
                margin-bottom: 30px;

                img{
                    height: 30px;
                    margin-right: 10px;
                }

                div{
                    h6{
                        margin-bottom: 5px;
                    }

                    p{
                        font-size: 11px;
                        color: $tundoraColor;
                    }
                }
            }
        }
    }

    .awards{
        text-align: center;

        h5{
            font-size: 15px;
            margin-bottom: 30px;
        }
        .awards-container{
            display: flex;
            justify-content: space-around;

            .my_awards-container{
                margin: 0 20px;

                img{
                    width: 85px;
                }

                .text{
                    margin: 10px 0;
                    font-size: 11px;
                    font-weight: bold;
                    line-height: 1.8;
                    color: $tundoraColor;
                }
            }
        }
    }
}
</style>


.my_awards-container{
    margin: 0 20px;

    img{
        width: 80px;
    }

    .text{
        margin: 10px 0;
        font-size: 11px;
        font-weight: bold;
        line-height: 1.8;
        color: $tundoraColor;
    }
}
