<template>
  <div>
      <div class="marketing-ressources-container">
        <div class="top-resources-section">
          <h2>Marketing Resources: Insider Advice On How to Increase Online Sales</h2>

          <div class="my_btn-container">
              <a href="#" class="my_resources-btn">Explore All Resources</a>
          </div>
        </div>

          <div class="my_card">
            <MarketingResourcesComponent v-for="(info, index) in marketinginfo"
            :key="index"
            :img="info.img"
            :text="info.text" />
          </div>
      </div>
  </div>
</template>

<script>
import MarketingResourcesComponent from "./SubMainComponents/MarketingResourcesComponent.vue"


export default {
    name: 'MarketingResources',
    data(){
        return{
            marketinginfo: [
              {
                img: require("../../assets/img/blog-posts-6-200x133.jpg"),
                text: "Marketing Tips And Tricks For Your Website"
              },
              {
                img: require("../../assets/img/blog-posts-5-200x133.jpg"),
                text: "How to Write Stunning Blog Post Titles"
              },
              {
                img: require("../../assets/img/blog-posts-4-200x133.jpg"),
                text: "Techniques to Reduce Facebook Ads Spend"
              }
            ]
        }
    },
    components: {
      MarketingResourcesComponent
    }
}
</script>

<style lang="scss" scoped>
@import "../../assets/global.scss";

.marketing-ressources-container{
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  margin: 0 auto;
  width: 65%;
  padding: 80px 20px;

    .top-resources-section{
      display: flex;
      justify-content: space-between;
      align-items: flex-end;

      h2{
        font-size: 30px;
        margin-bottom: 60px;
        width: 45%;
      }

      .my_btn-container{
          height: 100%;
          display: flex;
          margin-bottom: 60px;
          
          .my_resources-btn{
              padding: 10px 25px;
              color: $whiteColor;
              background-color: $ecstasyColor;
              border-radius: 5px;
              text-decoration: none;
          }
      }
    }

    .my_card{
      display: flex;
      justify-content: center;
      width: 21%;
    }
}
</style>