<template lang="pug">
.curso-main-container.introduccion
  BannerInterno
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5.mb-5.bg-intro
    .titulo-principal.color-acento-contenido
      .titulo-principal__numero
        span
          i.fas.fa-info
      h1 Introducción
    .row.justify-content-center
      .col-lg-9.mb-lg-0.mb-3
        p.mb-4 Para generar los estados financieros de propósito general, es indispensable realizar el cierre contable, cuyo objetivo es reflejar el saldo correcto de las cuentas. En dado caso que se presenten diferencias, se deben realizar los respectivos asientos de ajuste.
        .row.justify-content-center.g-0
          .col-lg-6.col-7.mb-lg-0.mb-3: img(src='@/assets/curso/temas/1.png', alt='')
          .col-lg-6

            .p-4(style='background-color: #FEEAD4').h-100
                h3.text-center.text-md-start Nota aclaratoria: 
                p.mb-0.text-center.text-md-start
                    | Las tablas que se toman como referencia en los ejemplos en cada uno de los temas desarrollados, elaboradas mediante el programa Excel, son derivadas de los mismos; por lo tanto, no se numeran y la elaboración es propia del autor del presente componente.
      .col-lg-3.col-7: img(src='@/assets/curso/temas/2.png', alt='')

</template>

<script>
export default {
  name: 'Introduccion',
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

<style lang="sass">
.bg-intro
  background-image: url('../assets/curso/temas/bg-intro.png')
  background-size: cover
  background-position: center
  background-repeat: no-repeat
  position: relative
</style>
