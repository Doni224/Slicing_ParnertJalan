<template>
  <div>
    <ol>
        <li > Makan 3 Kali</li>
        <li>Pemandu Wisata</li>
        <li>Brosur atau peta</li>
        <li>Transportasi</li>
        <li>Wi-fi Gratis</li>
        <li>Penyewaan Perlengkapan</li>
        <li>Audio Guide</li>
    </ol>
  </div>
</template>

<script>
import axios from 'axios';
export default {
    data(){
    return{
      fasilitastour:[],
      pathTour: this.$pathApi
    }
  },
  methods: {
    setFasilitasTour(data) {
      this.fasilitastour = data;
    },
  },
  name: "FasilitasTour",
  props: ["tour"],
  mounted() {
    axios
      .get(this.pathTour + "api/user/fasilitasuser/tour", {
        headers: {
          'ngrok-skip-browser-warning': 1
        }
      })
      .then((response) => this.setFasilitasTour(response.data))
      .catch((error) =>
        console.log("gagal :", error));
  },
}
</script>

<style>

</style>