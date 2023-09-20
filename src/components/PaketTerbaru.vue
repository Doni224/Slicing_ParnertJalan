<template>
  <div id="app">
    <div class="con container">
      <h2 class="title" data-aos="fade-up" data-aos-duration="1000">Paket Wisata terbaru untuk kamu</h2>
      <br />
      <carousel  
        :items="1"
        :loop="true"
        :autoplay="true"
        :margin="30"
        :nav="false"
        :dots="true"
        :animateOut="fadeOut"
        :animateIn="fadeIn"
        :autoplayHoverPause="false"
        :responsive="{
          0: {
            items: 1.5,
          },
          500: {
            items: 2,
          },
          768: {
            items: 3,
          },
          1000: {
            items: 4,
          },
        }"
      >
      <div class="carousel"  data-aos="fade-up" data-aos-duration="1000" data-aos-delay="50">
            <h3 class="carousel-text" data-aos="fade-up" data-aos-duration="1000" data-aos-delay="50" >Paket Wisata <br />Dieng</h3>
            <button class="carousel-btn btn btn-primary" data-aos="fade-up" data-aos-duration="1000" data-aos-delay="100">
              <router-link class="nav-link" > </router-link> Lihat Detail
            </button>
            <div class="carousel-bg"></div>
            <img class="carousell-img" src="../assets/img/dieng.png" alt />
          </div>
          <div class="carousel"  data-aos="fade-up" data-aos-duration="1000" data-aos-delay="50">
            <h3 class="carousel-text" data-aos="fade-up" data-aos-duration="1000" data-aos-delay="50" >Paket Wisata <br />Purwokerto</h3>
            <button class="carousel-btn btn btn-primary" data-aos="fade-up" data-aos-duration="1000" data-aos-delay="100">
              <router-link class="nav-link" > </router-link> Lihat Detail
            </button>
            <div class="carousel-bg"></div>
            <img class="carousell-img" src="../assets/img/pwt.png" alt />
          </div>
          <div class="carousel"  data-aos="fade-up" data-aos-duration="1000" data-aos-delay="50">
            <h3 class="carousel-text" data-aos="fade-up" data-aos-duration="1000" data-aos-delay="50" >Paket Wisata <br />Semarang</h3>
            <button class="carousel-btn btn btn-primary" data-aos="fade-up" data-aos-duration="1000" data-aos-delay="100">
              <router-link class="nav-link" > </router-link> Lihat Detail
            </button>
            <div class="carousel-bg"></div>
            <img class="carousell-img" src="../assets/img/semarang.png" alt />
          </div>
          <div class="carousel"  data-aos="fade-up" data-aos-duration="1000" data-aos-delay="50">
            <h3 class="carousel-text" data-aos="fade-up" data-aos-duration="1000" data-aos-delay="50" >Paket Wisata <br />Lombok</h3>
            <button class="carousel-btn btn btn-primary" data-aos="fade-up" data-aos-duration="1000" data-aos-delay="100">
              <router-link class="nav-link" > </router-link> Lihat Detail
            </button>
            <div class="carousel-bg"></div>
            <img class="carousell-img" src="../assets/img/lombok.png" alt />
          </div>
      </carousel>
    </div>
  </div>
</template>

<script>
import carousel from "vue-owl-carousel";
//import WisataRekomend from "./wisata/WisataRekomend.vue";
export default {
  name: "DaftarWisata",
  components: {
    carousel,
   //WisataRekomend
},

};
</script>

<style>

.carousel {
  position: relative;
  border-radius: 20px;
  overflow: hidden;
  height: 300px;
  
}
.carousel-text {
  position: absolute;
  bottom: 0;
  margin-bottom: 100px;
  margin-left: 20px;
  z-index: 551;
  color: #ffffff;
}
.carousel-btn {
  position: absolute;
  bottom: 0;
  z-index: 9999;
  margin-left: 20px;
  margin-bottom: 40px;
}
.carousel-bg {
  width: 100%;
  position: absolute;
  bottom: 0;
  height: 100%;
  background: linear-gradient(transparent, #000000);
  opacity: 0.8;
  z-index: 550;
}
.carousel-img {
  height:100%;
}
</style>
