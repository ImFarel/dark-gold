<template>
  <div class="bridename container-fluid pt-5 pb-5">
      <!-- Vector Bunga -->
      <img src="../assets/images/BrideNameImg/bunga3.png" id="bunga1" class="mt-5">
      <img src="../assets/images/BrideNameImg/bunga4.png" id="bunga2" class="mt-5">
      <div class="bridename-content mt-3">
        <div class="bn-text text-center container">
          <p>Assalamu'alaikum Warahmatullahi Wabarakatuh.</p>
          <p>Maha suci Allah yang telah menciptakan mahluk-Nya berpasang-pasangan. Ya Allah, 
              perkenankanlah kami merangkaikan kasih sayang yang Kau ciptakan <br> diantara kami untuk 
              mengikuti Sunnah Rasul-Mu dalam rangka membentuk keluarga yang sakinah, mawaddah, warahmah.
          </p>
        </div>

        <div class="bn-mempelai container d-flex justify-content-center">
            <div class="mempelai-pria">
                <div class="foto-pria">
                    <img src="../assets/images/BrideNameImg/ftpria.png" alt="Foto Pria">
                </div>
                <div class="nama-mempelai">
                    <div class="nama">
                        <h1>Azrial</h1>
                    </div>
                    <div class="sub-nama">
                        <p>Putra pertama dari keluarga <br> Bapak Abiyyu dan Ibu Anggraeni</p>
                    </div>
                </div>
            </div>
            <div class="memp-text text-center mx-7">
                <p>dengan</p>
            </div>
            <div class="mempelai-wanita">
                <div class="foto-wanita">
                    <img src="../assets/images/BrideNameImg/ftwnta.png" alt="Foto Wanita">
                </div>
                <div class="nama-mempelai">
                    <div class="nama">
                        <h1>Razlina </h1>
                    </div>
                    <div class="sub-nama">
                        <p>Putri kedua dari keluarga <br> Bapak Adrian dan Ibu Tsania</p>
                    </div>
                </div>
            </div>
        </div>
      </div>
  </div>
</template>

<script>
export default {
    name: 'BrideName',
}
</script>

<style>
    .bridename {
        min-height: 100vh;
        background: linear-gradient(296.55deg, rgba(0, 0, 0, 0.9) 2.36%, rgba(18, 19, 23, 0.846) 99.37%);
        position: relative;
    }

    #bunga1, #bunga2 {
        position: absolute;
        top: 0;
    }

    .bridename img#bunga1 {
        left: 0;
    }

    .bridename img#bunga2 {
        right: 0;
    }

    #bunga1, #bunga2 {
        z-index: -1;
    }

/* === bridename Text Pembukaan === */
    .bn-text {
        color: var(--primary-color);
        padding: 1rem;
    }

    .bn-text p {
        font-family: var(--second-font);
        font-style: italic;
        font-weight: 400;
        font-size: 15px;
    }

    .mempelai-pria {
        height: 300px;
    }

/* === Menambahkan Vector disamping bawah masing-masing foto mempelai === */
    .mempelai-pria .foto-pria {
        background: url("../assets/images/BrideNameImg/Vector 4.png");
    }

    .mempelai-wanita .foto-wanita {
        background: url("../assets/images/BrideNameImg/Vector 3.png");
        transform: translateX(.5rem);
    }

    .mempelai-pria .foto-pria,
    .mempelai-wanita .foto-wanita {
        background-size: 130px;
        background-repeat: no-repeat;
        background-position: bottom center;
        width: 150px;
        padding: 1rem;
    }

/* === Atur Size Foto Pengantin (Mobile) === */
    .mempelai-pria .foto-pria img, 
    .mempelai-wanita .foto-wanita img {
        max-width: 110px;
    }

/* === CSS untuk teks dengan diantara foto pengantin === */
    .memp-text {
        height: 180px;
        display: flex;
        align-items: center;
    }

    .memp-text p {
        font-family: var(--third-font);
        font-style: italic;
        color: var(--primary-color);
    }

/* === CSS Nama mempelai (Azrial & Razlina) === */
    .nama-mempelai {
        margin-top: 2rem;
    }

    .nama h1 {
        color: var(--white);
        text-align: center;
        font-family: var(--first-font);
        padding-bottom: 1rem;
    }

/* === Sub Nama (Putra/i dari keluarga ... ) */
    .sub-nama p {
        color: var(--white);
        text-align: center;
        font-family: var(--second-font);
    }
    /* === Iphone 5/SE === */
    @media screen and (max-width: 3220px) and (max-height: 568px) {
        .mempelai-pria .foto-pria,
        .mempelai-wanita .foto-wanita {
            background-size: 100px;
            background-position: bottom  left;
            width: 00%;
        }

        .mempelai-pria .foto-pria img, 
        .mempelai-wanita .foto-wanita img {
            max-width: 70px;
            object-fit: cover;
        }

        .mempelai-wanita .foto-wanita {
            transform: translateX(0);
        }
    }

/* === Desktop Ver === */
    @media screen and (min-width: 900px) {
        .mempelai-pria .foto-pria img, 
        .mempelai-wanita .foto-wanita img {
            max-width: 210px;
        }

        .mempelai-pria .foto-pria,
        .mempelai-wanita .foto-wanita {
            background-size: 230px;
            background-repeat: no-repeat;
            background-position: bottom center;
            width: 250px;
            padding: 1rem;
        }

        .memp-text {
            height: 300px;
        }
    }

    @media screen and (min-width: 1200px) {
        #bunga1, #bunga2 {
            z-index: 1;
        }
    }
</style>    