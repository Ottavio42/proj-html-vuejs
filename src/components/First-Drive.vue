<template>
  <section class="first-drive">
      <div class="first-drive-cont">
          <div class="mettiti-al-volante">
              <h2>Get behind the wheel</h2>
              <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Veniam dolore quam sapiente, ab porro quos eligendi dicta praesentium provident error itaque recusandae molestiae enim laudantium, consequatur cumque quibusdam fugit quae.
              </p>
              <span>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Consectetur ut placeat inventore esse fugiat aliquid maiores, cum laudantium eius sunt a fugit quia voluptate atque? Ipsa, cum dolorum. Soluta, sint! Lorem ipsum, dolor sit amet consectetur adipisicing elit. Atque totam nisi enim quibusdam odio autem omnis pariatur itaque laboriosam perspiciatis soluta aspernatur nemo, vero reiciendis, iure aliquam consequuntur cumque. Quam.</span>
          </div>
          <div class="reg-prima-lezione">
            <div class="reg-prima-lezione-cont">
              <h2>First Lesson Free!</h2>
              <span>When u make a block booking with us your first lesson is included free</span>
              <form action="/action_page.php">
              <input type="text" class="pInfo"  name="name" placeholder="Name*"><br>
              <input type="email" class="pInfo"  name="email" placeholder="Email*"><br>
              <input type="tel"   class="pInfo" name="phone" placeholder="Telephone"><br>
              <input type="text"  class="pInfo" name="city" placeholder="Location"><br>
              <input type="submit" class="btn-verde" value="Request a call back">
              </form>
            </div>
          </div>
      </div>
  </section>
</template>

<script>
export default {
  name: "FirstDrive",
};
</script>

<style lang="scss" scoped>
@import "../assets/style/variables.scss";
.first-drive-cont{
  display: flex;
  padding: 2rem 0;
  width: $sizeCont;
  margin: auto;
  h2{
    color: $mainColor;
  }
  .mettiti-al-volante, .reg-prima-lezione{
    width: 50%;
    span{
      font-size: .75rem;
      color: #bbcbd3;
    }
    p{
      color: #bbcbd3;
    }
    p, h2{
      padding-bottom: .9375rem;
    }

  }
  .mettiti-al-volante{
    margin-right: .9375rem;
    h2{
      color: #494c4e;
    }
    
  }
  .reg-prima-lezione{
    text-align: center;
   position: relative;

   
   .reg-prima-lezione-cont{
     position: absolute;
     bottom: 3rem;
     background-color: #fff;
     padding: .625rem;
     border-radius: .625rem;
     box-shadow:  
              -5px -5px 3px #dedede,
               5px -5px 3px #dedede,
              -5px  5px 3px #dedede;
   }
    .pInfo{
      width: 80%;
      margin-top: .9375rem;
      height: 1.875rem;
    }
    .btn-verde{
      padding: 5px 12px;
      background-color: $mainColor;
      border-radius: 10px;
      color: #fff;
      font-size: 1.25rem;
      font-weight: 500;
      margin-top: .9375rem;
    }

  }

}
</style>