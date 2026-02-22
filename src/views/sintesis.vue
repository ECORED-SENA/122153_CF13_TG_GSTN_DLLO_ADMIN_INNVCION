<template lang="pug">
.curso-main-container.pb-3
  BannerInterno(icono="fas fa-sitemap" titulo="Síntesis")
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5

    p.mb-5 El siguiente mapa integra los criterios y especificidades de los conocimientos expuestos en el presente componente formativo:
    
    .row.justify-content-center
      .col-lg-12.mb-5
        figure
          img(src="@/assets/curso/temas/sintesis.svg", alt="A continuación, se presenta la síntesis del componente formativo: Los archivos y valoración documental conta de: Las nuevas tecnologías y su aplicación a la gestión documental con soportes electrónicos (hardware y software) y redes, correo electrónico, internet e intranet. El soporte informático como medio documental con obsolescencia, perdurabilidad y conservación, confiabilidad- seguridad y protección, legalidad. Preservación documental digital con duración corta, media y larga. Normativa de SST y sus elementos de protección personal y normas de gestión ambiental. Valoración y transferencia documental con sus tablas de transferencia documental y transferencias documentales.")
      .col-auto
        a.anexo.mb-4(:href="obtenerLink('/downloads/Sintesis.pdf')" target="_blank")
          .anexo__icono
            img(src="@/assets/template/icono-pdf.svg")
          .anexo__texto
            p Anexo. Síntesis

</template>

<script>
export default {
  name: 'Sintesis',
  data: () => ({
    // variables de vue
  }),
  mounted() {
    this.$nextTick(() => {
      this.$aosRefresh()
    })
  },
  updated() {
    this.$aosRefresh()
  },
}
</script>

<style lang="sass"></style>
