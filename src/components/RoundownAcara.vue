<template>
  <div class="roundown-acara container-fluid text-center">

      <div class="roundown-content container text-center py-5">
        <div class="tanggal-countdown mb-4">
          <div class="tc-title m-auto">
                <!-- Vector Bunga -->
                <img src="../assets/images/RoundownAcaraImg/bunga2.png" alt="Bunga" id="bunga22">
                <img src="../assets/images/RoundownAcaraImg/bunga1.png" alt="Bunga" id="bunga11">
              <h2 v-if="!expired">Rangkaian Acara Akan Diselenggarakan</h2>
              <h2 v-else>Acara Sedang/Sudah Berlangsung</h2>
          </div>
          <div class="tanggal-acara pt-3">
              <h1>{{ tanggal }}</h1>
          </div>

          <div class="countdown container mt-5" v-if="loaded">

              <div class="countdown-wrapper row d-flex justify-content-center">

                <div class="box-date col-lg-1 col-3 mx-3 p-5" id="box-hari">
                    <h2>{{ displayDays }}</h2>
                    <span>Hari</span>
                </div>

                <div class="box-date col-lg-1 col-3 mx-3 p-5" id="box-jam">
                    <h2>{{ displayHours }}</h2>
                    <span>Jam</span>
                </div>

                <div class="box-date col-lg-1 col-3 mx-3 p-5" id="box-menit">
                    <h2>{{ displayMinutes }}</h2>
                    <span>Menit</span>
                </div>

                <div class="box-date col-lg-1 col-3 mx-3 p-5" id="box-detik">
                    <h2>{{ displaySeconds }}</h2>
                    <span>Detik</span>
                </div>
              </div>
          </div>
        </div>

        <div class="info-acara p-3 m-auto">
            <!-- /* === Vector Bunga Di Setiap Ujung Sisi === */-->
            <img src="../assets/images/RoundownAcaraImg/b1.png" alt="Bunga" id="b1">
            <img src="../assets/images/RoundownAcaraImg/b2.png" alt="Bunga" id="b2">
            <img src="../assets/images/RoundownAcaraImg/b3.png" alt="Bunga" id="b3">
            <img src="../assets/images/RoundownAcaraImg/b4.png" alt="Bunga" id="b4">

            <div class="info-acara-wrapper row d-flex justify-content-center w-100">

                <div class="kolom-info col-lg-5 col-md-12 p-3" id="kolom-info-satu">
                    <div class="akad-nikah text-center pb-1">
                        <h1 class="kolom-title">Akad Nikah</h1>
                        <h6 class="kolom-subtitle">Sabtu 12 Desember 2022</h6>
                        <p class="kolom-subtitle">08.00 WIB - Selesai</p>
                    </div>
                    <div class="lokasi pt-1">
                        <h1 class="kolom-title">Lokasi</h1>
                        <p class="kolom-subtitle">Masjid Al-Ikhlas</p>
                        <div class="maps-location w-70 d-flex justify-content-around m-auto">
                            <div class="g-maps map-link m-1">
                                <a href="#">Gmaps</a>
                            </div>
                            <div class="maze map-link m-1">
                                <a href="#">Maze</a>
                            </div>
                        </div>
                    </div>
                </div>

                <div class="kolom-info col-lg-5 col-md-12 p-3" id="kolom-info-dua">
                    <div class="resepsi-nikah text-center pb-1">
                        <h1 class="kolom-title">Resepsi Nikah</h1>
                        <h6 class="kolom-subtitle">Minggu 13 Desember 2022</h6>
                        <p class="kolom-subtitle">09.00 WIB - Selesai</p>
                    </div>
                    <div class="lokasi pt-1">
                        <h1 class="kolom-title">Lokasi</h1>
                        <p class="kolom-subtitle">Kediaman Mempelai Wanita</p>
                        <div class="maps-location w-70 d-flex justify-content-around m-auto ">
                            <div class="g-maps map-link m-1">
                                <a href="#">Gmaps</a>
                            </div>
                            <div class="maze map-link m-1">
                                <a href="#">Maze</a>
                            </div>
                        </div>
                    </div>
                </div>

            </div>

        </div>

 </div>

        <div class="container-fluid align-items-center m-auto d-flex flex-column mt-4">
            <div class="m-auto">
                 <img class="card-img-top" src="../assets/images/RoundownAcaraImg/bunga.png">
            </div>
            <div class="kata-story">
                <p >Tidak ada yang spesial dalam cerita kami. Tapi kami sangat spesial untuk satu sama lain. Dan <br>
                Kami bersyukur, dipertemukan Allah diwaktu terbaik, kini kami menanti hari istimewa kami.</p>
            </div>

            <div class="foto-pasangan d-flex flex-wrap justify-content-center align-items-center">

                    <img  src="../assets/images/RoundownAcaraImg/WeddingKit-3.png"  alt="">

                    <img  src="../assets/images/RoundownAcaraImg/WeddingKit-2.png"  alt="">

                    <img  src="../assets/images/RoundownAcaraImg/WeddingKit-1.png"  alt="">
            </div>
        </div>

        <div class="img-cerita-kami">
            <img  src="../assets/images/img/Group28.png"  alt="">
        </div>

        <div class="d-flex justify-content-center mt-4">
            <div class=" bg-transparent col-md-4 mx-3 mt-4">
                <div class="margin-top-title-3 title-story">
                    <p class="kolom-title text-end" id="tanggal">16 Juli 2013</p>
                    <p class="text-end" id="ket">Pertemuan pertama</p>
                 </div>

                <div class="card-story card-story-2 margin-top-card-story bg- rounded">
                    <div class="rounded item-story bg-light  d-flex flex-column">
                        <p class="kolom-title ms-2 text-dark me-auto  " id="judul">Acara Lamaran</p>
                        <img src="../assets/images/RoundownAcaraImg/WeddingKit-2.png" id="img" alt="">
                        <p class="text-dark ms-2 text-start " id="ket">Setelah 6 tahun bersama kami memutuskan untuk
                            melanjutkan ke hubungan yang lebih serius.
                        </p>
                    </div>
                </div>
                <div class="title-story margin-top-title-2">
                    <p class="kolom-title text-end" id="tanggal">18 Agustus 2021</p>
                    <p class="text-end" id="ket">Pernikahan</p>
                 </div>
            </div>

            <div class="pemisah-story">
                   <img  src="../assets/images/img/garis.png"  alt="">
            </div>

            <div class="  col-md-4 ms-3 mt-5">
                <div class="card-story bg- rounded margin-top-card-story-3">
                    <div class="rounded item-story bg-light  d-flex flex-column">
                        <p class="kolom-title ms-2 text-dark me-auto  " id="judul">Awal Bertemu</p>
                        <img src="../assets/images/RoundownAcaraImg/WeddingKit-3.png"  id="img" alt="">
                        <p class="text-dark ms-2 text-start " id="ket">Awal pertama kenal si dia itu satu jurusan di kampus.</p>
                    </div>
                </div>
                <div class="title-story margin-top-title-1">
                    <p class="kolom-title text-start" id="tanggal">2 Januari 2019</p>
                    <p class="text-start" id="ket">Lamaran</p>
                 </div>
                   <div class="card-story margin-top-card-story-2 bg- rounded">
                    <div class="rounded item-story bg-light  d-flex flex-column">
                        <p class="kolom-title ms-2 text-dark me-auto  " id="judul">Awal Bertemu</p>
                        <img src="../assets/images/RoundownAcaraImg/WeddingKit-1.png"  id="img" alt="">
                        <p class="text-dark ms-2 text-start " id="ket">Akhirnya kami pun mengucapkan janji suci.</p>
                    </div>
                </div>

            </div>

        </div>

  </div>
</template>

<script>
export default {
  name: 'RoundownAcara',
  props: {
    tanggal: String,
  },
  data: () => ({
    displayDays: 0,
    displayHours: 0,
    displayMinutes: 0,
    displaySeconds: 0,
    loaded: false, // Agar Ketika di Refresh, Countdown Tidak Berubah Jadi 00:00:00:00
    expired: false, // Mengatur jika waktu countdown sudah habis
  }),
  computed: {
    _seconds: () => 1000,
    _minutes() {
      return this._seconds * 60;
    },
    _hours() {
      return this._minutes * 60;
    },
    _days() {
      return this._hours * 24;
    },
  },
  mounted() {
    this.showRemaining();
  },
  methods: {
    formatNum: (num) => (num < 10 ? `0${num}` : num), // Format Untuk Mendisplay Date
    showRemaining() {
      const timer = setInterval(() => {
        const date = new Date(); // Mengambil Date
        const dateEnd = new Date(2022, 11, 12, 10, 10, 10, 10); // Atur Countdown
        const distance = dateEnd.getTime() - date.getTime(); // Mencari jarak detik antara tanggal yang ditentukan dan tanggal sekarang

        if (distance < 0) { // Jika waktu countdown sudah habis, clearInterval Timer
          clearInterval(timer);
          this.expired = true;
          this.loaded = true;
          return;
        }

        const days = Math.floor((distance / this._days));
        const hours = Math.floor((distance % this._days) / this._hours);
        const minutes = Math.floor((distance % this._hours) / this._minutes);
        const seconds = Math.floor((distance % this._minutes) / this._seconds);

        this.displaySeconds = this.formatNum(seconds);
        this.displayMinutes = this.formatNum(minutes);
        this.displayHours = this.formatNum(hours);
        this.displayDays = this.formatNum(days);
        this.loaded = true;
      }, 1000);
    },
  },
};
</script>

<style>

    .item-story{
            padding: 0.4rem;
        }
    .img-cerita-kami img{
        height: 100px;
        margin-top: 2rem;
    }
    .card-story {
        height: 26rem;
    }

    .item-card{
        height: 20rem;
    }

    .card-story #judul{
        font-size: 2rem;
    }
    .card-story #img{
        height: 240px;
        width: auto;
    }
    .card-story #ket{
        font-size: 20px;
    }

    .margin-top-card-story{
        margin-top: 25rem;
    }
    .margin-top-card-story-2{
        margin-top: 26.5rem;
    }
    .margin-top-card-story-3{
        margin-top: 0.6rem;
    }
     .margin-top-title-1{
        margin-top: 0rem;
    }
      .margin-top-title-2{
        margin-top: 1.7rem;
    }

    .foto-pasangan img{
        padding: 4px;
        max-width: 170px;

    }
    .kata-story p{
        color:white ;
        font-size: 8px;
        margin-top: 1rem;
        margin-bottom: 1rem;

    }

    .title-story #tanggal{
        font-size: 40px;

    }

    .title-story #ket{
        font-size: 20px;
        margin-top: -20px;

    }

    .roundown-acara {
        min-height: 100vh;
        background: #222121;
        color: var(--white);
        font-weight: 400;
        position: relative;
        padding-bottom: 5rem;
    }

    .roundown-acara #vec-bunga {
        position: absolute;
        bottom: 0;
        left: 0;
        max-width: 100%;
    }

    .tanggal-countdown .tc-title h2 {
        font-size: 15px;
        font-family: var(--second-font);
    }

    .tc-title {
        width: 350px;
        position: relative;
    }

    /* === Vector Bunga Kecil Di Samping TC Title === */
    #bunga11, #bunga22 {
        position: absolute;
        max-width: 50px;
        transform: translateY(-1rem);
    }

    #bunga11 { right: 0; }
    #bunga22 { left: 0 }

    @media screen and (max-width: 768px) {
        .tc-title { width: 100%; }
        #bunga11 { right: -5% }
        #bunga22 { left: -5% }
    }

    .tanggal-acara h1 {
        font-family: var(--first-font);
        color: var(--primary-color);
        font-size: 32px;
    }

    .box-date {
        height: 90px;
        background: rgba(54, 47, 45, 0.7);
        border-radius: 11px;
        border: 3px solid var(--primary-color);
        display: flex;
        justify-content: center;
        align-items: center;
        flex-direction: column;
        margin-bottom: 2rem;
    }

    .box-date h2 {
        font-family: var(--first-font);
    }

    .box-date span {
        font-family: var(--second-font);
        letter-spacing: 1px;
    }

    /* === Kotak Info Acara === */
    .info-acara {
        width: 70%;
        height: 600px;
        background: rgba(54, 47, 45, 0.7);
        border: 5px solid var(--primary-color);
        border-radius: 11px;
        display: grid;
        place-items: center;
        position: relative;
    }

    /* === Vector Bunga Di Setiap Ujung Sisi === */
    .info-acara img {
        position: absolute;
        max-width: 130px;
    }

    #b1, #b2 {
        top: 1%;
    }

    #b3, #b4 {
        bottom: 1%;
    }

    #b1, #b3 {
        left: 2%;
    }

    #b2, #b4 {
        right: 2%;
    }

    #kolom-info-satu {
        border-right: 1px solid var(--primary-color);
    }

    #kolom-info-dua {
        border-left: 1px solid var(--primary-color);
    }

    /* === CSS Untuk Isi dari Kolom Info === */
    .kolom-title {
        font-family: var(--first-font);
        color: var(--primary-color);
    }
    .akad-nikah h6, .resepsi-nikah h6 {
        color: var(--primary-color);
    }
    .kolom-subtitle {
        font-family: var(--second-font);
    }

    .maps-location .map-link {
        width: 150.39px;
        background: rgba(104, 90, 85, 0.7);
        border: 1px solid #EECC98;
        box-sizing: border-box;
        border-radius: 30px;
    }

    .maps-location .map-link a {
        text-decoration: none;
        color: var(--white);
        font-family: var(--second-font);
        font-weight: normal;
    }

    @media screen and (max-width: 768px) {
        .info-acara {
            width: 100%;
            height: 100%;
        }

        /* === Menghilangkan Border === */
        #kolom-info-satu {
            border-right: none;
        }

        #kolom-info-dua {
            border-left: none;
        }

        /* === Maps Button === */
        .maps-location {
            flex-direction: column;
            justify-content: center;
        }

        .maps-location .map-link {
            width: 100%;
        }

        /* === Menyesuaikan Size Vector === */
        .info-acara img {
            max-width: 50px;
        }

        .lokasi {
            margin-bottom: 3rem;
        }

          .img-cerita-kami img {
            height: 50px;
        }

        .pemisah-story img{
            height: 35rem;
        }
        .title-story{
            margin-top: -20px;
        }
        .title-story #tanggal{
        font-size: 20px;

        }

        .title-story #ket{
            font-size: 10px;
            margin-top: -20px;
        }

        .card-story {
            height: 10rem;
            margin-top: -1.7rem;
            width: 10rem;
        }
        .card-story-2 {
            height: 10rem;
            width: 9.2rem;
        }
        .item-story{
            padding: 0.4rem;
        }
        .card-story #judul{
            font-size: 1.2rem;
            margin-bottom: -0.12rem;
        }
        .card-story #img{
            height: 80px;
            width: auto;
        }

        .card-story #ket{
            font-size: 10px;
            margin-bottom: -0.1rem;
        }

        .margin-top-card-story{
            margin-top: 9.2rem;
        }
        .margin-top-card-story-2{
            margin-top: 10.1rem;

        }
        .margin-top-title-1{
            margin-top: 0.8rem;
        }
        .margin-top-title-2{
            margin-top: 1.8rem;
        }
        .margin-top-title-3{
             margin-top: -0.8rem;
        }

      }

    @media screen and (min-width: 992px) {
        .roundown-acara {
            padding-bottom: 15rem;
        }

        .foto-pasangan img{
              max-width: 30rem;
        }

        .kata-story p{
            font-size: 30px;
            margin-bottom: 2rem;
            margin-top: 0;
        }
    }

</style>
