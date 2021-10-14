<template>
  <section class="hero">
    <div class="hero-cont">
      <div class="hero-text">
        <h1>Drive with Avada</h1>
        <p>We offer the finest driving tutorial money can buy</p>
      </div>
      <div class="hero-button">
        <a href="#">
          <span><i class="fas fa-id-card-alt"></i></span>
          <div>Demos</div>
        </a>
        <a href="#">
          <span id="btn-verde">$39</span>
          <div>On sale</div>
        </a>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Hero",
};
</script>

<style lang="scss" scoped>
@import "../assets/style/variables.scss";
.hero{
  height: 500px;
  background-image: url("../assets/img/homepage-hero-background.jpg");
  background-size: cover;
  position: relative;
  z-index: 0;
  .hero-cont{
    width: $sizeCont;
    margin: auto;
    height: 100%;
    display: flex;
    align-items: center;
    .hero-text{
      color: #fff;
      h1{
        font-size: 1.875rem;
      }
      p{
        font-size: 1.25rem;
      }
    }
    .hero-button{
      position: absolute;
      right: 1rem;
      top: 10rem;
      a{
        display: block;
        text-decoration: none;
        color: #33475b;
        background-color: #fff;
        border-radius: .625rem;
        text-align: center;
        margin-bottom: .625rem;
        font-size: .75rem;
        padding: .3125rem;
        span{
          font-size: 1.25rem;
        }
      }
      #btn-verde{
            color: $mainColor;
          }
    }
  }

}

</style>