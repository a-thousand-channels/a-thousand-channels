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
   .text-white {
    color:  white;
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

   .column h4 .emoji {
      background: none;
      -webkit-text-fill-color: black;
   }
   .column h4 svg {
      display: inline-block;
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
   button svg {
     display: inline;
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
      background-size: 100% 0.3em;
      background-position: 0 100%;
    }
    .bg-a100c-1-button {
        background: none;
        background-color: rgba(242, 71, 38, 1);
        background: -webkit-linear-gradient(120deg,rgba(255,0,35,.75),rgba(255,117,0,.75) 50%,rgba(255,0,249,.75));
     }
    .bg-a100c-2-button {
        background: none;
        background-color: rgba(242, 71, 38, 1);
        background: -webkit-linear-gradient(70deg,rgba(255,0,35,.75),rgba(255,117,0,.75) 50%,rgba(255,0,249,.75));
    }
    .bg-a100c-3-button {
        background: none;
        background-color: rgba(242, 71, 38, 1);
        background: -webkit-linear-gradient(10deg,rgba(255,0,35,.75),rgba(255,117,0,.75) 50%,rgba(255,0,249,.75));
    }
    h1 {
      @apply pb-0 pt-1 pl-5 pr-5 text-2xl md:text-3xl font-semibold leading-8
    }
    h3 {
      @apply pb-4 pt-4 pl-5 pr-5 text-3xl  font-semibold
    }
    h4 {
      @apply pb-0 pt-0 pl-5 pr-0 text-3xl font-light
    }

    .column h4 {
      @apply text-xl font-bold
    }
    p {
      @apply pb-2 pt-2 pl-5 pr-5
    }
    p.small {
      @apply text-sm
    }
    .column p {
      @apply pb-2 pt-2 pl-8 pr-5
    }
    div.lang_ar h1,
    div.lang_ar h2,
    div.lang_ar h3,
    div.lang_ar h4,
    div.lang_ar ul,
    div.lang_ar ol,
    div.lang_ar ul li,
    div.lang_ar ol li,
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
      max-width: 1200px;
      border-top-color: rgba(255,0,35,.75);
      margin: 22px auto;
      opacity: 0;
    }
    video {
      max-width: 100%;
      /* 100% made old safaris very confused */
      height: unset;
    }
    img.illustration.illustration-middle {
      @apply py-6 px-4 mx-auto w-[125px] lg:w-[125px]
    }
    img.illustration.illustration-left {
      @apply py-6 px-4 mx-auto w-[300px] mt-[35px] lg:absolute lg:ml-[-150px] lg:mt-[30px] lg:w-[270px] rotate-[-25deg]
    }
    img.illustration.illustration-left1 {
      @apply py-6 px-4 mx-auto w-[300px] mt-[35px] lg:absolute lg:ml-[-220px] lg:mt-[5px] lg:w-[270px]
    }
    img.illustration.illustration-left2 {
      @apply py-6 px-4 mx-auto w-[300px] mt-[35px] lg:absolute lg:ml-[-100px] lg:mt-[60px] lg:w-[240px] rotate-[-5deg]
    }
    img.illustration.illustration-left3 {
      @apply py-6 px-4 mx-auto w-[300px] mt-[35px] lg:absolute lg:ml-[-100px] lg:mt-[60px] lg:w-[200px] rotate-[-5deg]
    }
    img.illustration.illustration-right {
      @apply py-6 px-4 mx-auto w-[250px] mt-[35px] lg:absolute lg:ml-[600px] lg:mt-[25px] lg:w-[340px]
    }
    img.illustration.illustration-right1 {
      @apply py-6 px-4 mx-auto w-[300px] mt-[50px] lg:absolute lg:ml-[550px] lg:mt-[50px] lg:w-[320px]
    }
    img.illustration.illustration-right2 {
      @apply pt-12 pb-4 px-4 mx-auto w-[185px] lg:absolute lg:ml-[670px] lg:mt-[50px] lg:w-[240px]
    }
    img.illustration.illustration-right3 {
      @apply pt-12 pb-4 px-4 mx-auto w-[185px] lg:absolute lg:ml-[670px] lg:mt-[50px] lg:w-[190px]
    }
    img.illustration.illustration-outside-left {
      @apply pt-12 pb-6 px-4 mx-auto w-[200px] lg:block lg:absolute lg:ml-[-125px] lg:mt-[385px] lg:w-[190px]
    }
    img.illustration.illustration-outside-left1 {
      @apply pt-12 pb-6 px-4 mx-auto w-[200px] lg:block lg:absolute lg:ml-[-125px] lg:mt-[85px] lg:w-[190px]
    }
    img.illustration.illustration-outside-right {
      @apply hidden py-6 px-4 mx-auto w-[200px] lg:block lg:absolute lg:ml-[710px] lg:mt-[545px] lg:w-[190px]
    }
    div.block {
      @apply overflow-hidden shadow sm:rounded-md p-6 mt-5
    }
    div.block.large {
      @apply overflow-hidden shadow sm:rounded-md text-lg p-6 mt-5
    }
    div.block.block-after-illustration {
      @apply lg:mt-[170px]
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
      @apply md:flex text-sm pt-4 pb-0
    }
    div.block-3
     {
      @apply md:flex text-sm pt-4 pb-4
    }
    div.column {
      background-color: white;
    }
    div.block .column p {
      @apply pb-2 pt-2 pl-5 pr-5
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
      <div class="flex max-h-[650px] lg:max-h-[650px] xl:max-h-[650px] 2xl:max-h-[700px]">
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
            v-if="locale.active == true"
            :key="locale.code"
            :to="switchLocalePath(locale.code)"
            class="text-link2 mr-2 px-1 pb-1 font-semibold drop-shadow-sm shadow-black text-white">
            {{ locale.code }}
          </nuxt-link>

        </div>
      </div>

      <div class="mt-8 bg-white overflow-hidden shadow p-6">
        <h1 class="lang_ar" v-if="$i18n.locale == 'ar'">
          ألف وسيلة - منصة  🎁 لرسم و خلق الخرائط 🌎  الكويرية <img src="~/assets/lgbtq+_rainbow_flag_quasar_progress_flag_variant.svg" class="h-6 inline p-0 pb-1 align-middle" title="Pride flag variant based on Daniel Quasar's 2018 design combining elements of the Philadelphia flag and the trans pride flag, and brown and black." alt="Pride flag variant based on Daniel Quasar's 2018 design combining elements of the Philadelphia flag and the trans pride flag, and brown and black.">
        </h1>
        <h1 v-else>
          A Thousand Channels –  {{ $t('project_part1') }} <img src="/progresiveflagcolor.svg" style="height: 30px; display: inline;" title="Pride flag variant based on Daniel Quasar's 2018 design combining elements of the Philadelphia flag and the trans pride flag, and brown and black." alt="Pride flag variant based on Daniel Quasar's 2018 design combining elements of the Philadelphia flag and the trans pride flag, and brown and black."> {{ $t('project_part2') }}
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

</div>

<div v-if="$i18n.locale == 'es'">

    <nuxt-content :document="index_es" />


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
      draft_index_de: [],
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
    this.index_es = await this.$content('index_es', { deep: true }).fetch()
  }

}

</script>
