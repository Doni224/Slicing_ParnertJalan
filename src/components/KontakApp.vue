

<template>
  <div class="container kontak">
    <div class="kontakTitle">
      <h2 class="title" data-aos="fade-up" data-aos-duration="1000">Kontak Kami</h2>
      <p class="title-kontak" data-aos="fade-up" data-aos-duration="1000" data-aos-delay="50">
        Hubungi kami, jika ingin paket wisata secara custom <br />
        atau ada pertanyaan terkait layanan kami.
      </p>
    </div>
    <div class="kontakL row">
      <div class="col-sm-6 col-12 kont">
      
        <h3 class="title-hubungi" data-aos="fade-up" data-aos-duration="1000" data-aos-delay="50">Hubungi kami melalui</h3>
        <div class="d-flex">
          <KontakUs />
        </div>
      </div>
      <div class="col-sm col-5 kontak2">
       
        <div class="row"><MediaSosial />
          </div>
      </div>
    </div>
  </div>
</template>

<script>
import KontakUs from "./Kontak/KontakUs.vue";
import MediaSosial from "./Kontak/MediaSosial.vue";
//import MediaSosial from "./Kontak/MediaSosial.vue";


export default {
  components: { KontakUs, MediaSosial },
};
</script>

<style>
.heading-kontak{
  font-family: 'Lato', sans-serif;
  font-weight: bold;
  line-height: 43px;
  font-style: normal;
}
.title-kontak{
    font-family: 'Roboto', sans-serif;
    font-weight: 400;
}
.title-hubungi{
    font-family: 'Lato', sans-serif;
    font-weight: bold;
    font-size: 24px;
  }
</style>