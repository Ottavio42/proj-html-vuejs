<template>
  <section class="courses">
      <div class="contact-us">
          <div class="cu-cont">
              <div class="cu-text">
                  <h2>Star learning to drive today</h2>
                  <p>Give us a call to schedule your first driving lesson</p>
              </div>
              <div class="cu-phone">
                   <div><i class="fas fa-phone"></i> 1-800-555-555</div>
              </div>
          </div>
      </div>
      <div class="courses-type">
          <div class="ct-cont">
              <div class="ct-info">
                  <div class="ct-info-cont">
                      <h2>Courses</h2>
                      <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Voluptates omnis est et numquam. Iusto quod blanditiis doloribus consequatur dignissimos, omnis ut deleniti maxime ipsum, excepturi quos, quae numquam repellendus a?</p>
                      <a href="#"> Course information</a>
                  </div>
              </div>
              <div class="ct-type">
                  <div class="type-card">
                      <img src="../assets/img/courses-passplus.jpg" alt="course-passplus">
                      <h3>Pass Plus</h3>
                      <a href="#">LEARN MORE</a>
                  </div>
                  <div class="type-card">
                      <img src="../assets/img/course-intensive.jpg" alt="course-intensive">
                      <h3>Intensive</h3>
                      <a href="#">LEARN MORE</a>
                  </div>
                  <div class="type-card">
                      <img src="../assets/img/courses-instructor.jpg" alt="course-instructor">
                      <h3>Instructor</h3>
                      <a href="#">LEARN MORE</a>
                  </div>
              </div>
          </div>
      </div>
  </section>
</template>

<script>
export default {
  name: "Courses",
};
</script>

<style lang="scss" scoped>
@import "../assets/style/variables.scss";
.courses{
    .contact-us{
        height: 11rem;
        background-image: url("../assets/img/horizontal-cta-background.jpg");
        background-size: cover;
        .cu-cont{
            width: $sizeCont;
            margin: auto;
            display: flex;
            align-items: center;
            height: 11rem;
            .cu-text, .cu-phone{
                width: 50%;
                color: #fff;
            }
        }
    }
    .courses-type{
        height: 22rem;
        background-image: url("../assets/img/promise-background.jpg");
        background-size: cover;
         background-repeat: no-repeat;
        background-position: bottom;
        .ct-cont{
            display: flex;
            width: 70%;
            margin: auto;
            .ct-info{
                position: relative;
                width: 40%;
                .ct-info-cont{
                    background-color: #fff;
                    position: absolute;
                    bottom: 6rem;
                    padding: .625rem;
                    border-radius: .625rem;
                    box-shadow:5px 5px 3px #dedede;
                    text-align: center;
                    h2, p{
                        padding: 1rem;
                    }
                    a{
                        display: block;
                        padding: 5px 12px;
                        background-color: $mainColor;
                        border-radius: 10px;
                        color: #fff;
                        font-weight: 500;
                        text-decoration: none;
                        margin: 1rem 1rem 2rem 1rem;
                    }
                    
                }
            }
            .ct-type{
                display: flex;
                width: 60%;
                .type-card{
                    padding: 3rem 0 1.25rem 1.25rem;
                    h3{
                        color: #7799ad;
                        text-align: center;
                    }
                    a{
                        display: block;
                        padding: 5px 12px;
                        background-color: #fff;
                        border-radius: 1.25rem;
                        border: .1875rem solid #7799ad;
                        color: #7799ad;
                        text-align: center;
                        font-weight: 700;
                        text-decoration: none;
                        margin: 1rem 1rem 2rem 1rem;
                    }
                    img{
                        width: 100%;
                        padding-bottom: .625rem;
                    }
                }
            }
        }
    }
}

</style>