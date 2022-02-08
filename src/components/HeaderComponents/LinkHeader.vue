<template>
  <div>
      <div class="my_container">
        <div class="my_link-container" v-for="(element, index) in links"
        :key="index">
            <a :href="element.href">{{element.text}}</a>
        </div>
      </div>
  </div>
</template>

<script>
export default {
    name: 'LinkHeader',
    data(){
      return{
        links: [
          {
            text: "Home",
            href: "#"
          },
          {
            text: "Services",
            href: "#"
          },
          {
            text: "Why Us",
            href: "#"
          },
          {
            text: "Case Studies",
            href: "#"
          },
          {
            text: "About",
            href: "#"
          },
          {
            text: "Blog",
            href: "#"
          }
        ]
      }
    }
}
</script>

<style lang="scss" scoped>
@import "../../assets/global.scss";

.my_container{
    height: 100%;
    display: flex;
    align-items: center;

    .my_link-container{
        padding: 0 15px;
        text-align: center;

        a{
            text-decoration: none;
            color: $blackColor;
            padding: 5px;

            &:hover{
                color: $ecstasyColor;
                border-bottom: 2px solid $ecstasyColor;
            }
        }
    }
}
</style>