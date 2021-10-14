<template>
  <header>
    <div class="header-top">
      <div class="header-top-cont">
        <div>We have a 95% Succesfull pass Rate!</div>
        <div><i class="fas fa-phone"></i> Give us a call to back your tutorial 1-800-555-555</div>
      </div>
    </div>
    <div class="header-bot">
      <div class="header-bot-cont">
        <img :src="require('../assets/img/' + logo)">
        <nav>
          <ul>
            <li v-for="(link, index) in headerNav" :key="index">
              <a href="#">{{ link }}</a>
            </li>
          </ul>
        </nav>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  name: 'Header',
  props: ["headerNav"],
  data(){
    return{
      logo: "logo-driving.png",
    };
  },
};
</script>


<style scoped lang="scss">
@import "../assets/style/variables.scss";
header{
  height: 10rem;
  width: 100%;
  position: fixed;
  z-index: 1;
  top: 0;
  right: 0;
  //header-top
  .header-top{
    background-color: #353637;
    color: #bbcbd3;
    .header-top-cont{
      width: $sizeCont;
      margin: auto;
      display: flex;
      justify-content: space-between;
      align-items: center;
      height: 3rem;
    }
  }
  //header-bot
  .header-bot{
    background-color: rgba(53, 54, 55, 0.5);
    color: #fff;
    .header-bot-cont{
      width: $sizeCont;
      margin: auto;
      display: flex;
      justify-content: space-between;
      align-items: center;
      height: 7rem;
      img{
        height: 3rem;
      }
      ul{
        display: flex;
        list-style: none;
        li{
          padding-left: 2rem;
          a{
            text-decoration: none;
            color: #fff;
            font-size: 1.25rem;
            font-weight: 700;
          }
        }
      }
      ul li:last-child a{
        padding: 5px 12px;
        background-color: $mainColor;
        border-radius: 10px;
      }
    }
  }
}
</style>
