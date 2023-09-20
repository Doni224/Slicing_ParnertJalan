<template>
  <div class="mypartnership">
    <div class="container"  >
      <h2 class="title" data-aos="fade-up" data-aos-duration="1000">Partnership Kami</h2>

      <carousel  
        :items="1"
        :loop="true"
        :autoplay="true"
        :margin="20"
        :nav="false"
        :dots="false"
        :animateOut="fadeOut"
        :animateIn="fadeIn"
        :autoplayHoverPause="false"
        :responsive="{
          0: {
            items: 2,
          },
          768: {
            items: 3,
          },
          1000: {
            items: 5,
          },
        }"
      > 
        <div class="patnerbox">
            <div class="card" style="padding:21px;border:none" data-aos="fade-up" data-aos-duration="1000" data-aos-delay="50">
              <div class="d-flex align-items-center" style="height:100px;">
                <img class="card-img-top" src="../assets/img/Partnert/dwidaya.png" alt="">
              </div>
            </div>
        </div>
        <div class="patnerbox">
            <div class="card" style="padding:21px;border:none" data-aos="fade-up" data-aos-duration="1000" data-aos-delay="50">
              <div class="d-flex align-items-center" style="height:100px;">
                <img class="card-img-top" src="../assets/img/Partnert/Hayu.png" alt="">
              </div>
            </div>
        </div>
        <div class="patnerbox">
            <div class="card" style="padding:21px;border:none" data-aos="fade-up" data-aos-duration="1000" data-aos-delay="50">
              <div class="d-flex align-items-center" style="height:100px;">
                <img class="card-img-top" src="../assets/img/Partnert/mister.png" alt="">
              </div>
            </div>
        </div>
        <div class="patnerbox">
            <div class="card" style="padding:21px;border:none" data-aos="fade-up" data-aos-duration="1000" data-aos-delay="50">
              <div class="d-flex align-items-center" style="height:100px;">
                <img class="card-img-top" src="../assets/img/Partnert/trave.png" alt="">
              </div>
            </div>
        </div>
        <div class="patnerbox">
            <div class="card" style="padding:21px;border:none" data-aos="fade-up" data-aos-duration="1000" data-aos-delay="50">
              <div class="d-flex align-items-center" style="height:100px;">
                <img class="card-img-top" src="../assets/img/Partnert/salsa.png" alt="">
              </div>
            </div>
        </div>
      </carousel>
    </div>
  </div>
</template>
  
  <script>
import carousel from "vue-owl-carousel";

export default {
  name: "DaftarWisata",
  components: {
    carousel,
  },
 
};
</script>
  
<style>

</style>
  