<style>

   .bg-a100c-1 {
      background: rgb(255,0,249);
      background: linear-gradient(90deg, rgba(255,0,249,0.25) 0%, rgba(255,117,0,0.25) 50%, rgba(255,0,35,0.25) 100%);
   }
   .bg-a100c-2 {
      background: rgb(255,0,249);
      background: linear-gradient(90deg, rgba(255,117,0,0.15) 0%, rgba(255,0,35,0.15) 50%, rgba(255,0,249,0.15) 100% );
   }
   .bg-a100c-3 {
      background: rgb(255,0,249);
      background: linear-gradient(90deg, rgba(255,0,35,0.15) 0%, rgba(255,0,249,0.15) 50%, rgba(255,117,0,0.15) 100% );
   }
   .text-a100c-1, .column h4 {
      font-size: 1.55rem;
      color: #ff6d6d;
      background: -webkit-linear-gradient(120deg,rgba(255,0,35,.75),rgba(255,117,0,.75) 50%,rgba(255,0,249,.75));
      -webkit-background-clip: text;
      background-clip: text;
      -webkit-text-fill-color: transparent;
      /* transform: rotate(-1.5deg); */
   }
   .column:first-child h4 {
      /* transform: rotate(2.5deg); */
   }
   .column:last-child h4 {
       /* transform: rotate(2deg); */
   }
    .bg-white {
      background-color: white;
     }
   .text-gray-800 {
    color:  #676767;
   }
    button.text-link,
    a.text-link {
      text-decoration: none;
      background-image: linear-gradient(120deg, #fde68a 0, #fde68a 100%);
      background-repeat: no-repeat;
      background-size: 100% 0.4em;
      background-position: 0 100%;
    }
    button.text-link,
    a.text-link2 {
      text-decoration: none;
      background-image: linear-gradient(120deg, #fde68a 0, #fde68a 100%);
      background-repeat: no-repeat;
      background-size: 100% 0.2em;
      background-position: 0 100%;
    }
    h1 {
      @apply pb-0 pt-1 pl-5 pr-5 text-2xl md:text-3xl font-light leading-8
    }
    h3 {
      @apply pb-4 pt-4 pl-5 pr-5 text-3xl font-normal
    }
    h4 {
      @apply pb-0 pt-0 pl-5 pr-5 text-2xl font-light
    }
    .column h4 {
      @apply text-2xl font-bold
    }
    p {
      @apply pb-2 pt-2 pl-5 pr-5
    }
    div.lang_ar h1,
    div.lang_ar h2,
    div.lang_ar h3,
    div.lang_ar h4,
    div.lang_ar ul,
    div.lang_ar ul li,
    div.lang_ar p
    {
      direction:  rtl;
    }
    h1.lang_ar {
      direction:  rtl;
    }

    ol {
      padding: 0.5rem 2.25rem 0.5rem 3.25rem;
      counter-reset: my-awesome-counter;
      margin: 1rem 3rem 0;
    }
    ol li {
      margin: 0 0 1rem 0;
      counter-increment: my-awesome-counter;
      position: relative;
    }

    ol li::before {
      content: counter(my-awesome-counter);
      color: #ffffff;
      font-size: 1.5rem;
      font-weight: normal;
      position: absolute;
      --size: 32px;
      left: calc(-1 * var(--size) - 15px);
      line-height: var(--size);
      width: var(--size);
      height: var(--size);
      top: -2px;
      transform: rotate(0);
      background: -webkit-linear-gradient(120deg,rgba(255,0,35,.75),rgba(255,117,0,.75) 50%,rgba(255,0,249,.75));
      border-radius: 50%;
      text-align: center;
      box-shadow: 0 1px 3px 0 rgba(0, 0, 0, 0.1), 0 1px 2px 0 rgba(0, 0, 0, 0.06)
    }
    ol li::before {
      /* content: none; */
    }
    div.lang_ar ol li::before {
      left: auto;
      right:  calc(-1 * var(--size) - 15px);;
    }

    hr {
      max-width: 400px;
      border-top-color: rgba(255,0,35,.75);
      margin: 22px auto;
    }
    video {
      max-width: 100%;
      /* 100% made old safaris very confused */
      height: unset;
    }
    div.block {
      @apply overflow-hidden shadow sm:rounded-sm p-6 mt-5
    }
    div.block.large {
      @apply overflow-hidden shadow sm:rounded-sm text-lg p-6 mt-5
    }
    div.block {
      background-color: white;
    }
    div.block-1
     {
      @apply md:flex text-sm pt-4 pb-4 px-4 md:px-16
    }
    div.block-2
     {
      @apply md:flex text-sm pt-4 pb-4
    }
    div.block-3
     {
      @apply md:flex text-sm pt-4 pb-4
    }
    div.column {
      background-color: white;
    }
    div.block-1 .column {
      @apply  md:flex-1
    }
    div.block-1 .column h4 {
      @apply px-2 py-2 md:p-2
    }
    div.block-1 .column p {
      @apply px-2 py-2 md:p-2
    }
    div.block-2 .column {
      @apply  md:flex-1 pb-5
    }
    div.block-2 .column h3 {
      @apply py-1 px-5  md:py-1 md:px-5
    }
    div.block-2 .column p {
      @apply py-1 px-5  md:py-1 md:px-5
    }
    div.block-3 .column {
      @apply  md:flex-1
    }
    div.block-3 .column p {
      @apply p-5 md:p-5
    }
    div.block-2 .column:first-child,
    div.block-3 .column:first-child {
      @apply md:mr-2
    }
    div.block-2 .column:last-child,
    div.block-3 .column:last-child {
      @apply md:ml-2
    }

  </style>

<template>
<div id="page">
  <div class="relative flex bg-white bg-a100c-1 min-h-[200px] items-top justify-center sm:items-center sm:pt-0">
      <div class="flex max-h-[650px] lg:max-h-[750px] lg:mt-[-80px] xl:max-h-[800px] 2xl:max-h-[800px]">
        <video class="" autoplay loop muted  playsinline poster="https://github.com/a-thousand-channels/a1000c-assets/blob/main/aThousandChannels_Animation_Banner.jpg?raw=true">
          <source src="https://github.com/a-thousand-channels/a1000c-assets/blob/main/aThousandChannels_Animation_Banner.mp4?raw=true" type="video/mp4">
          Your browser does not support the video tag.
        </video>
      </div>
  </div>
  <div class="relative flex items-top justify-center min-h-screen bg-a100c-1 sm:items-center sm:pt-0">

    <div class="max-w-4xl mx-auto px-6 lg:px-12 mt-[-60px] sm:mt-[-90px] md:mt-[-105px] lg:mt-[-120px]">
      <div class="flex">
        <div class="flex align-center justify-center pl-10 sm:pt-0 mr-auto ml-[-54px] lg:ml-[-110px]">
          <img src="~/assets/a-thousand-channels--logo-variant-a--short.png" title="A thousand channels" class="mb-[-58px] md:mb-[-64px] lg:mb-[-64px] w-16 md:w-24 lg:w-28">
        </div>
        <div class="flex justify-right ml-auto mt-auto mb-[-25px] px-2">

         <nuxt-link
            v-for="locale in $i18n.locales"
            :key="locale.code"
            :to="switchLocalePath(locale.code)"
            class="text-link2 mr-2 px-1">
            {{ locale.code }}
          </nuxt-link>

        </div>
      </div>

      <div class="mt-8 bg-white overflow-hidden shadow p-6">
        <h1 class="lang_ar" v-if="$i18n.locale == 'ar'">
          ألف وسيلة - منصة  🎁 لرسم و خلق الخرائط 🌎  الكويرية <img src="~/assets/lgbtq+_rainbow_flag_quasar_progress_flag_variant.svg" class="h-6 inline p-0 pb-1 align-middle" title="Pride flag variant based on Daniel Quasar's 2018 design combining elements of the Philadelphia flag and the trans pride flag, and brown and black." alt="Pride flag variant based on Daniel Quasar's 2018 design combining elements of the Philadelphia flag and the trans pride flag, and brown and black.">
        </h1>
        <h1 v-else>
          A Thousand Channels –  {{ $t('project_part1') }} <img src="~/assets/lgbtq+_rainbow_flag_quasar_progress_flag_variant.svg" class="h-6 inline p-0 pb-1 align-middle" title="Pride flag variant based on Daniel Quasar's 2018 design combining elements of the Philadelphia flag and the trans pride flag, and brown and black." alt="Pride flag variant based on Daniel Quasar's 2018 design combining elements of the Philadelphia flag and the trans pride flag, and brown and black."> {{ $t('project_part2') }}
        </h1>
      </div>

<div v-if="$i18n.locale == 'en'">

        <nuxt-content :document="index_en" />

</div>

<div v-if="$i18n.locale == 'ar'">

    <div class="lang_ar">
        <nuxt-content :document="index_ar" />
    </div>

</div>

<div v-if="$i18n.locale == 'de'" class="">

        <nuxt-content :document="index_de" />


        <div class="block-2">

          <div class="column">

              <img src="/fgtq_all_layers_dark.jpg" class="pb-1">

              <h3>Intersections & Constellations. From Gay to Queer</h3>

              <p>

              Seit Sommer 2021 arbeitet die Working group „Queer narratives, mapped“ mit unserer Plattform. <br>

              </p>
              <p>
              Aus dieser Zusammenarbeit ist die <a href="https://from-gay-to-queer.net/" class="text-link" target="_blank">Karte "From Gay to Queer"</a> entstanden, die mit dem zeitlichen Schwerpunkt in den 1990er Jahren und dem räumlichen Fokus auf Bremen erzählt, wie sich aus lesbischen und schwulen Nischen queere Kulturen und Bündnisse entwickelt haben. <br>
              </p>
              <p>
              Aus Interviews und der Sammlung von Flyern, Postern, Fotos und anderen Druckerzeugnissen ist eine Karte entstanden, die von unterschiedlichen, persönlichen Perspektiven auf die Entstehung von queeren Communities und Koalitionen erzählt.
              </p>
          </div>
          <div class="column">

              <img src="/fgtq_all_layers_dark.jpg" class="pb-1">

              <h3>„Queer.topia“: Eine reale Utopie in 12 Bildern</h3>

              <p>
              Seit Sommer 2021 arbeitet die Working group „Queer narratives, mapped“ mit unserer Plattform. <br>
              </p>
              <p>
              Aus dieser Zusammenarbeit ist die <a href="https://from-gay-to-queer.net/" class="text-link" target="_blank">Karte "From Gay to Queer"</a> entstanden, die mit dem zeitlichen Schwerpunkt in den 1990er Jahren und dem räumlichen Fokus auf Bremen erzählt, wie sich aus lesbischen und schwulen Nischen queere Kulturen und Bündnisse entwickelt haben. <br>
              </p>
              <p>
              Aus Interviews und der Sammlung von Flyern, Postern, Fotos und anderen Druckerzeugnissen ist eine Karte entstanden, die von unterschiedlichen, persönlichen Perspektiven auf die Entstehung von queeren Communities und Koalitionen erzählt.
              </p>
          </div>
        </div>

      </div>

      <div v-if="$i18n.locale == 'es'" class="mt-8 bg-white overflow-hidden shadow sm:rounded-smX p-6">
        <p class="mt-3 text-gray-800">
          <strong>{{ $t('hello') }}</strong>
        </p>
        <p class="mt-3 text-gray-800">
          <em>... Texto siguiente ...</em>
        </p>

      </div>
      <Footer></Footer>

    </div>
  </div>
</div>
</template>



<script>

export default {
  data() {
    return {
      index_de: [],
      index_en: [],
      index_es: [],
      index_ar: []

    }
  },
  methods: {
    scrollToTop() {
      window.scrollTo({ top: 0, behavior: 'smooth' })
    }
  },
  async fetch() {
    this.index_de = await this.$content('index_de', { deep: true }).fetch()
    this.index_en = await this.$content('index_en', { deep: true }).fetch()
    this.index_ar = await this.$content('index_ar', { deep: true }).fetch()
  }

}

</script>
