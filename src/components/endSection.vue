<template>
  <div class="end-section  text-center" >
      <div class="table-end-section container-fluid d-flex flex-column">
        <p id="judul" class="kolom-title">Doa Restu Anda Merupakan Karunia Yang Sangat Berarti Bagi Kami.</p>
        <p id="ket">Dan jika memberi adalah ungkapan tanda kasih anda, anda dapat memberi kado secara cashless dengan mengirim <br>
        amplop digital secara transfer pada akun di bawah ini :</p>
        <div class="d-flex justify-content-center flex-wrap">

              <div class="qr-code d-flex flex-column align-items-center">
                <p id="judul">BCA - 4980131187</p>
                <img src="../assets/images/img/Code1.png" alt="">
              </div>
              <div class="qr-code d-flex flex-column align-items-center">
                <p id="judul">OVO - 087780933640</p>
                <img src="../assets/images/img/Code2.png" alt="">
              </div>

        </div>

        <div class="d-flex end justify-content-center align-items-center">

            <img src="../assets/images/img/bunga10.png" alt="">
            <p class="kolom-title nama-pasangan">Agrial & Raglina</p>
            <img src="../assets/images/img/bunga11.png" alt="">
        </div>

      </div>
  </div>
</template>

<script>
export default {

};
</script>

<style>
    .end-section{
        min-height: auto;
        background: linear-gradient(296.55deg, rgba(0, 0, 0, 0.9) 2.36%, rgba(18, 19, 23, 0.846) 99.37%);
        color: var(--white);
        font-weight: 400;
        position: relative;
        padding-bottom: 5rem;
    }

    .table-end-section #judul{
        font-size: 3rem;
    }
     .table-end-section #ket{
        font-size: 1.4rem;
    }

    .qr-code{
        background: white;
        min-height: 20rem;
        min-width: 25rem;
        padding: 1rem;
        border-radius: 5px;
        color: black;
        display: grid;
        margin: 2rem;
    }

    .qr-code img{
        width: 13rem;
    }

    .qr-code #judul{
        font-size: 1.9rem;
    }

    .nama-pasangan{
        font-size: 6rem;
        margin-left: 1rem;
        margin-right: 1rem;
    }
    .end {
        margin-top: 3rem;
    }

     /* === CSS Untuk Isi dari Kolom Info === */
    .kolom-title {
        font-family: var(--first-font);
        color: var(--primary-color);
    }

    @media screen and (max-width: 768px) {
    .table-end-section #judul{
        font-size: 0.9rem;
        margin-top: 2rem;
    }
    .table-end-section #ket{
        font-size: 0.4rem;
        margin-top: -0.5rem;
    }

      .qr-code{
        min-height: 10rem;
        min-width: 9rem;
        padding: 0.5rem;
        border-radius: 2px;
        margin: 0.5rem;
    }
    .qr-code img{
        width: 7rem;
    }

    .qr-code #judul{
        margin-top: 0px;
        font-size: 0.8rem;
    }

     .nama-pasangan{
        font-size: 2rem;
        margin-left: 0.5rem;
        margin-right: 0.5rem;
    }
    .end img{

        max-height: 3rem;
    }
    .end{
        margin-top: 1rem;
    }
    }

</style>
