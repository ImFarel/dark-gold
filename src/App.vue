<template>
  <section-satu namaPria="Azrial" namaWanita="Razlina" />
  <bride-name />
  <roundown-acara tanggal="Sabtu, 15 Desember 2022"/>
  <buku-tamu-section/>
  <end-section/>
</template>

<script>
import SectionSatu from './components/SectionSatu.vue'
import BrideName from './components/BrideName.vue'
import RoundownAcara from './components/RoundownAcara.vue'
import BukuTamuSection from './components/bukuTamuSection.vue'
import EndSection from './components/endSection.vue'


export default {
  name: 'App',
  components: {
    SectionSatu,
    BrideName,
    RoundownAcara,
    BukuTamuSection,
    EndSection,
   
  }
}
</script>


<style>

</style>
