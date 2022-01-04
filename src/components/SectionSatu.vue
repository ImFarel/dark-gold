<template>
   <input type="checkbox" id="check">

        <div class="sidebar container-fluid p-2 d-flex justify-content-center align-items-center ">
            <div class="card-sidebar container">
                <div class="cover-text text-center rounded ">
                    <div class="header-side">
                        <p class="fs-3" >Undangan ernikahan</p>
                        <h1>{{ namaPria }} &  {{ namaWanita }}</h1>
                    </div>
                    <div class="footer-side">
                    <p class="fs-4 mt-2 ">Kpd Bpk/Ibu/Saudari/i <br>Nama Tamu Undangan</p>
                        <label for="check">
                            <i class="btn btn-primary" id="btn" >Buka Undangan</i>
                        </label>
                    </div>
                </div>
            </div>
        </div>

  <div class="cover container-fluid">
      <img src="../assets/images/SecImg/vector1.png" alt="Vector" id="vector1">
      <img src="../assets/images/SecImg/vector2.png" alt="Vector" id="vector2">
      <div class="cover-text  text-center">
          <p>The Wedding of</p>
          <h1>{{ namaPria }} <br> & <br> {{ namaWanita }}</h1>
      </div>
      <div class="cover-ayat text-center">
          <p>“Dan di antara tanda-tanda (kebesaran)-Nya adalah Dia menciptakan pasangan-pasangan
              untukmu dari jenismu sendiri, agar kamu cenderung dan merasa tenteram kepadanya,
              dan Dia menjadikan di antaramu rasa kasih dan sayang. Ar-Ruum : 21"
          </p>
      </div>
  </div
  >
</template>

<script>
export default {
  name: 'Cover',
  props: {
    namaPria: String,
    namaWanita: String,
  },
};
</script>

<style>
    @import url('https://fonts.googleapis.com/css2?family=Cabin:ital@0;1&family=EB+Garamond&family=Rochester&display=swap');

    * {
        margin: 0;
        padding: 0;
        box-sizing: border-box;
    }

    .card-sidebar {
        min-height: 85vh;
        background: url("../assets/images/Background/bg-flash-slide.png");
        display: grid;
        place-items: center;
        padding: 2rem;
        position: fixed;
        position: relative;
        z-index: 100;

    }

    .sidebar {
         min-height: 100vh;
         position: fixed;
         z-index: 90;
         background-color:rgb(0, 0, 0, 0.5);

    }

    label #btn{
        cursor: pointer;
    }

    #check{
        display: none;
    }

    #check:checked~.sidebar {
      top:-1000rem;
    }

     .cover {
        min-height: 100vh;
        background: url("../assets/images/SecImg/bgimage.png");
        display: grid;
        place-items: center;
        padding: 2rem;
        position: relative;
    }

    :root {
        --first-font: 'Rochester', cursive;
        --second-font: 'Cabin', sans-serif;
        --third-font: 'EB Garamond', serif;

        --primary-color: #EECC98;
        --white: #FFFFFF;
    }

    .container-flash{
        height: 100vh;
    }

    /* === Vector === */
    #vector1, #vector2 {
        position: absolute;
        height: 50vh
    }

    #vector1 {
        top: 5%;
        left: 3%;
    }

    #vector2 {
        bottom: 5%;
        right: 3%;
    }

    @media screen and (max-width: 768px) {
        #vector1, #vector2 {
            width: 50vw;
            height: 30vh;
        }
    }

/* === Menambahkan Overlay pada Background agar terlihat gelap === */
    .cover::after {
        content: '';
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        background: rgba(0, 0, 0, 0.336);
    }

    .cover-text p {
        font-family: var(--second-font);
        font-style: italic;
        font-size: 30px;
        color: var(--primary-color);
    }

    .cover-text h1 {
        font-family: var(--first-font);
        font-weight: 400;
        font-size: 70px;
        color: var(--white);
    }

    .cover-ayat {
        padding: .5rem;
    }

    .cover-ayat p {
        font-family: var(--second-font);
        font-size: 17px;
        color: var(--primary-color);
        font-weight: 400;
    }

    .cover-text, .cover-ayat {
        z-index: 1;
    }

    @media screen and (max-width: 992px) {
        .cover {
            background-size: cover;
            background-position: center;
        }
        .card-sidebar {
            background-size: cover;
            background-position: center;
        }
    }

    @media screen and (min-width: 992px) {
        .cover-text h1 {
            font-size: 80px;
        }

        .cover-ayat {
            padding: 0 10rem;
        }
    }
    @media screen and (max-width: 750px){
        .header-side{
            margin-top: 1rem;
        }
        .footer-side{
            margin-top: 14rem;
        }
    }
</style>
