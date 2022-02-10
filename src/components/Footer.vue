<template>
  <div>
    <div class="container-footer">
      <div class="top">
        <div class="top-footer-container">
          <div class="my_text-footer">
              <h1>
                  Let's Make Things Happen
              </h1>

              <p>Curabitur ac leo nunc. Vestibulum et mauris vel ante finibus maximus nec ut leo. Integer consectetur.</p>

              <div class="border-dot"></div>

              <p class="statement">"The team at Avada Marketing Consultant is fabulous. They helped us unlock our potential online and offline. We have experienced year on year growth due to thei progressive approach."</p>

              <p class="name">George Anderson</p>

              <p class="profession-role">Digitalbox CEO</p>
          </div>

          <div class="marketing-consultant-card">
              <MarketingConsultantExpertCard />
          </div>
        </div>

        <div class="bottom-footer-container">
          <div class="text-social-footer">
            <h6>Grow Your Online Business Strategically, and Improve Customer Retention.</h6>
            
              <div>
                <i v-for="(social, index) in socialicon"
                :key="index"
                :class="social"
                class="my_cursor"></i>
              </div>
          </div>

          <div class="links-container-footer">
            <div class="links-container" v-for="(link, index) in linkscontainer"
            :key="index"
          >
            <h5>{{link.heading}}</h5>

            <ul>
              <li v-for="(li, liindex) in link.link"
                :key="liindex"
              >
                <a href="#">{{li}}</a>
              </li>
            </ul>
          </div>
          </div>
        </div>
      </div>

      <div class="bottom">
        <div class="site-powered"><i class="fa-solid fa-copyright copyright"></i> <span>2020 Avada Consultant Powered by Wordpress</span></div>
        <div class="contact">
          <span>
            call Us (555) 802-1234
          </span>
          <span>
            info@yourcompany.com
          </span>
        </div>
      </div>

    </div>
  </div>
</template>

<script>
import MarketingConsultantExpertCard from './ReusableComponents/MarketingConsultantExpertCard.vue'

export default {
    name: 'Footer',
    data(){
      return{
        socialicon: [
          'fa-brands fa-facebook-f',
          'fa-brands fa-twitter',
          'fa-brands fa-instagram',
          'fa-brands fa-youtube',
          'fa-brands fa-linkedin-in',
          'fa-brands fa-tiktok'
        ],
        linkscontainer: [
          {
            heading: 'Services',
            link: [
              'Marketing Plan',
              'Sales Development',
              'Digital Marketing',
              'Pricing',
              'Why Us',
              'Case Studies'
            ]
          },
          {
            heading: 'Resources',
            link: [
              'Learning Center',
              'Video Tutorials',
              'Customers',
              'Blog'
            ]
          },
          {
            heading: 'Company',
            link: [
              'Who We Are',
              'Contact Us',
              'Careers'
            ]
          }
        ]
      }
    },
    components: {
      MarketingConsultantExpertCard
    }
}
</script>

<style lang="scss" scoped>
@import "../assets/global.scss";

.container-footer{
  display: flex;
  flex-direction: column;

  .top{
    .top-footer-container{
      height: 500px;
      background-color: $blackColor;
      position: relative;
      color: $whiteColor;
      display: flex;
      justify-content: center;
      align-items: center;

      .my_text-footer{
        width: 500px;
        position: absolute;
        top: 8%;
        left: 15%;

        h1{
            font-size: 50px;
            padding-bottom: 20px;
        }

        .border-dot{
          width: 100px;
          border: 1px solid $graynurseColor;
        }

        p{
            font-size: 20px;
            padding: 20px 0;
        }

        .statement{
          font-size: 18px;
          font-style: italic;
        }

        .name{
          font-size: 15px;
          font-weight: bold;
          padding-bottom: 0;
        }

        .profession-role{
          font-size: 9px;
          color: $graynurseColor;
          padding-top: 5px;
        }
      }

      .marketing-consultant-card{
              width: 300px;
              position: absolute;
              top: 8%;
              right: 21%;
      }
    }

    .bottom-footer-container{
      display: flex;
      justify-content: center;
      padding: 80px 0;

      .text-social-footer{
        width: 30%;
        padding-right: 150px;

        h6{
          font-size: 16px;
          margin-bottom: 30px;
        }

        div{
          width: 120px;
          display: flex;
          justify-content: space-between;
          
          .my_cursor{
            cursor: pointer;
          }
        }
      }

      .links-container-footer{
        width: 40%;
        display: flex;

        .links-container{
          width: 30%;

          h5{
            line-height: 2;
            margin-left: 24px;
          }

          ul{
            line-height: 2;
            li{
              list-style: none;

                a{
                  text-decoration: none;
                  color: $tundoraColor;
                }
              
            }
          }
        }
      }
    }
  }

  .bottom{
    display: flex;
    margin: 0 auto;
    width: 70%;

    .site-powered{
      width: 40%;

      span{
        font-size: 10px;
        color: $tundoraColor;
      }
    }

    .contact{
      width: 50%;
      display: flex;
      justify-content: space-between;
      margin-bottom: 80px;
      font-size: 12px;

      span{
        font-size: 10px;
        color: $tundoraColor;
      }
    }
  }
}  
</style>