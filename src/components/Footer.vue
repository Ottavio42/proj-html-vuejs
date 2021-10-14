<template>
    <footer>
        <div class="footer-top">
            <div class="footer-top-cont">
              <div class="info">
                  <img :src="require('../assets/img/' + logo)" alt="logo">
                  <p>Avada Driving School is the right choice for <br>
                   experieced drivers looking for a refresher <br>
                   course, or the brand new driver waiting to <br>
                   pass first time.</p>
              </div>
              <div class="details">
                  <h3>CONTACT DETAILS</h3>
                  <ul>
                      <li v-for="(info, index) in footerNav.information" :key= "index" >
                          <i :class="info.fawesome"></i>
                          <span> {{info.word}} </span>
                      </li>
                  </ul>
              </div>
              <div class="courses">
                  <h3>COURSES</h3>
                  <ul>
                      <li v-for="(course, index2) in footerNav.courses" :key= "index2">
                          <i class="fas fa-arrow-circle-right"></i>
                          <span> {{course}} </span>
                      </li>
                  </ul>
              </div>
              <div class="advertising">
                  <img :src="require('../assets/img/' + ad)">
                  <div>
                      <a href="#">BOOK NOW</a>
                  </div>
              </div>
            </div>
        </div>
        <div class="footer-bot">
            <div class="footer-bot-cont">
                <div class="copyright">© Copyright 2012-2020|Avada Theme by <span>Theme Fusion</span>| All Rights reserved|Powered by <span>WordPress</span> </div>
                <div class="social-icons">
                    <ul>
                        <li><i class="fab fa-facebook-f"></i></li>
                        <li><i class="fab fa-twitter"></i></li>
                        <li><i class="fab fa-youtube"></i></li>
                        <li><i class="fab fa-instagram"></i></li>
                    </ul>
                </div>
            </div>
        </div>
    </footer>
</template>

<script>
export default {
  name: 'Footer',
  props: ["footerNav"],
  data(){
    return{
      logo: "logo-driving.png",
      ad: "footer-ad-grid.png",
    };
  },
};
</script>
<style lang="scss" scoped>
@import "../assets/style/variables.scss";
//footer-top
.footer-top{
    color: #bbcbd3;
    background-color: #3b3f42;
    .footer-top-cont{
        display: flex;
        width: $sizeCont;
        height: 25rem;
        margin: auto;
        padding-top: 4rem;
        .info, .advertising{
            width: 30%;
            margin-left: 10px;
        }
        .details, .courses{
            width: 20%;
            margin-left: 10px;
            h3{
                color: #fff;
                font-size: 1.25rem;
                font-weight: 700;
                padding-bottom: .9375rem;
            }
        }
        .info img{
            height: 3rem;
            margin-bottom: 1rem;
        }
        .advertising img{
            height: 15rem;
            margin-bottom: 1rem;
        }
        .advertising {
            div{
                display: flex;
                justify-content: center;
                a{
                    padding: .3125rem .75rem;
                    background-color: #7abc64;
                    border-radius: .625rem;
                    text-decoration: none;
                    color: #fff;
                    font-size: 1.25rem;
                    font-weight: 700;
                }
            }
        }
        ul{
            list-style: none;
            li{
                display: flex;
                margin-bottom: 1rem;
                span{
                    margin-left: .3125rem;
                }
            }
        }
        .courses{
            ul{
                li{
                    color: #7abc64;
                }
            }
        }
    }
}
//footer-bottom
.footer-bot{
    background-color: #1c1d1e;
    color: #bbcbd3;
    .footer-bot-cont{
        display: flex;
        width: $sizeCont;
        height: 6rem;
        margin: auto;
        align-items: center;
        justify-content: space-between;
        .copyright{
            font-size: .625rem;
            span{
                color: #7abc64;
            }
        }
        .social-icons{
            ul{
                display: flex;
                list-style: none;
                li{
                    padding-left: 1rem;
                }
            }
        }
    }
}
</style>