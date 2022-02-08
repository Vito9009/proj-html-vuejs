<template>
  <div>
    <div class="my_contact-container">
        <i class="fa-solid fa-phone"></i>
        <span>(555) 802-1234</span>
    </div>
  </div>
</template>

<script>
export default {
    name: 'ContactHeader'
}
</script>

<style lang="scss" scoped>
@import "../../assets/global.scss";

.my_contact-container{
    height: 100%;
    width: 100px;
    display: flex;
    justify-content: space-between;
    align-items: center;

    .fa-phone{
      color: $ecstasyColor;
    }
}

</style>