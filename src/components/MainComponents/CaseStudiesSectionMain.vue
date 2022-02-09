<template>
  <div>
      <div class="card-organization-container">
          <h2>Trusted by Leading Organisations</h2>

          <div class="card">
            <CaseCardOrganization v-for="(info, index) in casestudiesinfo"
            :key="index"
            :img="info.img"
            :mainText="info.maintext"
            :text="info.text"
            :subText="info.subtext" />
          </div>

          <div class="my_btn-container">
              <a href="#" class="my_header-btn">Read More Case Studies</a>
          </div>
      </div>
  </div>
</template>

<script>
import CaseCardOrganization from "./SubMainComponents/CaseCardOrganization.vue"


export default {
    name: 'CaseStudiesSectionMain',
    data(){
        return{
            casestudiesinfo: [
              {
                img: require("../../assets/img/case-studies-1-600x675.jpg"),
                maintext: "How Spaces attracted five million visitors by improving the content",
                text: "200%",
                subtext: "Higher revenue from digital"
              },
              {
                img: require("../../assets/img/case-studies-4-600x675.jpg"),
                maintext: "Creativity helped Hemisferio to increase their brand reach vertically",
                text: "10x",
                subtext: "Sales increase with the same ad spend"
              },
              {
                img: require("../../assets/img/case-studies-6-600x675.jpg"),
                maintext: "How DigitalBox used AI-powered data insight to boost sales",
                text: "3-year",
                subtext: "Partnership with Avada Consultant"
              }
            ]
        }
    },
    components: {
      CaseCardOrganization
    }
}
</script>

<style lang="scss" scoped>
@import "../../assets/global.scss";

.card-organization-container{
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  margin: 0 auto;
  width: 75%;


    h2{
      font-size: 30px;
      margin: 60px 0;
    }

    .card{
      display: flex;
      justify-content: center;
      align-items: center;
      width: 21%;
    }

    .my_btn-container{
        height: 100%;
        display: flex;
        align-items: center;
        margin: 40px 0;
        
        .my_header-btn{
            padding: 10px 25px;
            color: $whiteColor;
            background-color: $ecstasyColor;
            border-radius: 5px;
            text-decoration: none;
        }
    }

}
</style>