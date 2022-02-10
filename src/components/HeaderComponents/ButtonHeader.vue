<template>
  <div>
    <div class="my_btn-container">
        <a href="#" class="my_header-btn">Free Quote</a>
    </div>
  </div>
</template>

<script>
export default {
    name: 'ButtonHeader'
}
</script>

<style lang="scss" scoped>
@import "../../assets/global.scss";

.my_btn-container{
    height: 100%;
    display: flex;
    align-items: center;
    
    .my_header-btn{
        padding: 10px 30px;
        color: $ecstasyColor;
        background-color: rgba(247, 98, 16, 0.2);
        border-radius: 5px;
        text-decoration: none;

        &:hover{
          color: $whiteColor;
          background-color: $ecstasyColor;
        }
    }
}
</style>