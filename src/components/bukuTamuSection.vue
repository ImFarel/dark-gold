<template>
<div class="buku-tamu-section text-center ">

    <div class="container-fluid  d-flex justify-content-center">
        <div class="bunga-left ">
            <img  src="../assets/images/img/Group30.png" alt="">
        </div>

        <div class="container-fluid d-flex form-buku-tamu">
            <div class="buku-tamu">
                <p id="judul" class="kolom-title text-end"> Buku Tamu</p>
                <p id="ket" class="text-end"> Berikan doa /Ucapan Terbaik Anda <br>
                kepada kedua  mempelai</p>
            </div>

            <div class="form-doa">
                    <div  id="border" >
                        <div class="p-form-doa d-flex rounded flex-column justify-content-evenly">
                            <form action="#" method="/POST">
                                <input class="form-control input-1" placeholder="Nama Anda" name="nama">
                                <textarea id="text-area-form" name="ket" class="form-control input-2" placeholder="Berikan Ucapan & Doa"></textarea>
                                <select  class="form-control" placeholder="Konfirmasi kehadiran" id="option-form" name="" >
                                    <option value="#" disabled selected>Konfirmasi Kehadiran</option>
                                    <option value="hadir">Hadir</option>
                                    <option value="tidak_hadir">Tidak Hadir</option>
                                </select>
                                <button id="button-form" type="submit"  class="btn">Kirim</button>
                            </form>
                        </div>
                    </div>
            </div>

        </div>

         <div class="bunga-right" >
            <img  src="../assets/images/img/Group29.png" alt="">
        </div>

    </div>

  </div>

</template>

<script>
export default {

};
</script>

<style>
    .buku-tamu-section {
        min-height: auto;
        padding-bottom: 2rem;
        background: linear-gradient(296.55deg, rgba(0, 0, 0, 0.9) 2.36%, rgba(18, 19, 23, 0.846) 99.37%);
        color: var(--white);
        font-weight: 400;
        position: relative;
    }
    .form-buku-tamu{
        z-index: 10;
        padding-left:4rem ;
        padding-right:7rem ;
        margin-top: 8rem;
    }

    .form-doa{
        min-width: 65rem;
        margin-left: 1rem;
    }
    .form-doa #border{
        border: 5px solid var(--primary-color);
        border-radius: 11px;
        background: rgba(54, 47, 45,9);

    }

    .form-doa input{
        margin: 1rem;
        border: 1px solid black;
        border-radius: 3px;

    }
    .form-doa .input-1{
        height: 2.5rem;
    }
     .form-doa .input-2{
        height: 4rem;
    }
     .form-doa .input-3{
        height: 2.5rem;
    }

    .form-doa #button-form{
        margin: 1rem;
        width: 5rem;
        background:var(--primary-color);
        border: 1px solid black;

    }

    .form-doa #option-form{
        margin: 1rem;
        border: 1px solid black;
        border-radius: 3px;

    }
    .form-doa #text-area-form{
        margin: 1rem;
        min-height: 8rem;
        border: 1px solid black;

    }
    .p-form-doa{
        padding:2rem ;
        box-sizing: border-box;
        background: white;
        margin: 2rem;
    }
    .bunga-left{
        margin-top: 15rem;
        left: 0;
        position: absolute;
    }
    .bunga-right{
        right: 0;
        position: absolute;

    }
    .buku-tamu{
        width: 16rem;

    }
    .buku-tamu #judul {
        font-size: 2rem;
    }
    .buku-tamu #ket {
        font-size: 1rem;
    }

    @media screen and (max-width: 768px)  {
    .bunga-left img{
        max-height: 4rem;
        margin-top: -17rem;

    }
    .bunga-right img{
        max-height: 4rem;

    }
    .form-buku-tamu{
        padding-left:2rem ;
        padding-right:2.5rem ;
        margin-top:3rem;
    }

    .buku-tamu{
        width: 7rem;
    }
    .buku-tamu #judul {
        font-size: 1.2rem;
    }
    .buku-tamu #ket {
        margin-top: -1rem;
        font-size: 0.45rem;
    }

    .form-doa{
        min-width: auto;
        margin-left: 0.5rem;
    }
     .p-form-doa{
        padding:0.6rem ;
        margin: 0.9rem;
        min-height: 15rem;
        width: 13rem;
    }

    .form-doa #border{
        border: 0.1rem solid var(--primary-color);
        border-radius: 3px;
        background: rgba(54, 47, 45,9);

    }
    .form-doa input{
        margin: 0.1rem;
        font-size: 12px;
        border: 1px solid black;
        border-radius: 1px;
    }
    .form-doa #text-area-form{
        margin: 0.1rem;
        font-size: 12px;
        min-height: 4rem;
        border: 1px solid black;
        border-radius: 1px;

    }
    .form-doa #option-form{
        margin: 0.1rem;
        font-size: 12px;
        border: 1px solid black;
        border-radius: 1px;

    }
    .form-doa #button-form{
        margin: 0.1rem;
        width:3rem;
        font-size: 0.5rem;
        background:var(--primary-color);
        border: 0.5px solid black
    }

    }
</style>
