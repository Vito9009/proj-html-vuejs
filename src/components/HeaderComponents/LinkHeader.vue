<template>
  <div>
      <div class="my_container">
        <div class="my_link-container" v-for="(element, index) in links"
        :key="index">
            <a :href="element.href" :class="{'active': element.clicked}">{{element.text}} <i class="down" :class="element.down"></i></a>
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
            href: "#",
            down: 'fa-solid fa-chevron-down',
            clicked: true
          },
          {
            text: "Services",
            href: "#",
            down: 'fa-solid fa-chevron-down',
            clicked: false
          },
          {
            text: "Why Us",
            href: "#",
            clicked: false
          },
          {
            text: "Case Studies",
            href: "#",
            clicked: false
          },
          {
            text: "About",
            href: "#",
            clicked: false
          },
          {
            text: "Blog",
            href: "#",
            clicked: false
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
        position: relative;
        display: inline-block;

        a{
            text-decoration: none;
            color: $blackColor;
            padding: 5px;

            &.active, &:hover{
                color: $ecstasyColor;
                border-bottom: 2px solid $ecstasyColor;
            }

            i{
              font-size: 9px;
              margin-left: 3px;
            }
        }
    }
}
</style>