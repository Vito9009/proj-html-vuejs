<template>
  <div>
    <div class="container-footer">
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
  </div>
</template>

<script>
import MarketingConsultantExpertCard from './ReusableComponents/MarketingConsultantExpertCard.vue'

export default {
    name: 'Footer',
    components: {
      MarketingConsultantExpertCard
    }
}
</script>

<style lang="scss" scoped>
@import "../assets/global.scss";

.container-footer{
  height: 500px;
  background-color: black;
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
</style>