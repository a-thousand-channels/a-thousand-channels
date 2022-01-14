<style>

    /* work-sans-regular - latin-ext_latin */
@font-face {
  font-family: 'Work Sans';
  font-style: normal;
  font-weight: 400;
  src: local(''),
       url('~/assets/fonts/worksans/work-sans-v13-latin-ext_latin-regular.woff2') format('woff2'), /* Chrome 26+, Opera 23+, Firefox 39+ */
       url('~/assets/fonts/worksans/work-sans-v13-latin-ext_latin-regular.woff') format('woff'); /* Chrome 6+, Firefox 3.6+, IE 9+, Safari 5.1+ */
}

/* work-sans-600 - latin-ext_latin */
@font-face {
  font-family: 'Work Sans';
  font-style: normal;
  font-weight: 600;
  src: local(''),
       url('~/assets/fonts/worksans/work-sans-v13-latin-ext_latin-600.woff2') format('woff2'), /* Chrome 26+, Opera 23+, Firefox 39+ */
       url('~/assets/fonts/worksans/work-sans-v13-latin-ext_latin-600.woff') format('woff'); /* Chrome 6+, Firefox 3.6+, IE 9+, Safari 5.1+ */
}

/* work-sans-800 - latin-ext_latin */
@font-face {
  font-family: 'Work Sans';
  font-style: normal;
  font-weight: 800;
  src: local(''),
       url('~/assets/fonts/worksans/work-sans-v13-latin-ext_latin-800.woff2') format('woff2'), /* Chrome 26+, Opera 23+, Firefox 39+ */
       url('~/assets/fonts/worksans/work-sans-v13-latin-ext_latin-800.woff') format('woff'); /* Chrome 6+, Firefox 3.6+, IE 9+, Safari 5.1+ */
}

/* work-sans-italic - latin-ext_latin */
@font-face {
  font-family: 'Work Sans';
  font-style: italic;
  font-weight: 400;
  src: local(''),
       url('~/assets/fonts/worksans/work-sans-v13-latin-ext_latin-italic.woff2') format('woff2'), /* Chrome 26+, Opera 23+, Firefox 39+ */
       url('~/assets/fonts/worksans/work-sans-v13-latin-ext_latin-italic.woff') format('woff'); /* Chrome 6+, Firefox 3.6+, IE 9+, Safari 5.1+ */
}

/* work-sans-600italic - latin-ext_latin */
@font-face {
  font-family: 'Work Sans';
  font-style: italic;
  font-weight: 600;
  src: local(''),
       url('~/assets/fonts/worksans/work-sans-v13-latin-ext_latin-600italic.woff2') format('woff2'), /* Chrome 26+, Opera 23+, Firefox 39+ */
       url('~/assets/fonts/worksans/work-sans-v13-latin-ext_latin-600italic.woff') format('woff'); /* Chrome 6+, Firefox 3.6+, IE 9+, Safari 5.1+ */
}

/* work-sans-800italic - latin-ext_latin */
@font-face {
  font-family: 'Work Sans';
  font-style: italic;
  font-weight: 800;
  src: local(''),
       url('~/assets/fonts/worksans/work-sans-v13-latin-ext_latin-800italic.woff2') format('woff2'), /* Chrome 26+, Opera 23+, Firefox 39+ */
       url('~/assets/fonts/worksans/work-sans-v13-latin-ext_latin-800italic.woff') format('woff'); /* Chrome 6+, Firefox 3.6+, IE 9+, Safari 5.1+ */
}
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
    .bg-white {
      background-color: white;
     }
   .text-gray-800 {
    color:  #888;
   }
    button.text-link,
    a.text-link {
      text-decoration: none;
      background-image: linear-gradient(120deg, #fde68a 0, #fde68a 100%);
      background-repeat: no-repeat;
      background-size: 100% 0.4em;
      background-position: 0 100%;
    }
    h1 {
      @apply pb-0 pt-1 pl-5 pr-5 text-2xl
    }
    h3, h4 {
      @apply pb-0 pt-4 pl-5 pr-5 font-semibold
    }
    p {
      @apply pb-2 pt-2 pl-5 pr-5
    }
    div.block {
      @apply overflow-hidden shadow sm:rounded-sm p-6 mt-8
    }
    div.block.large {
      @apply overflow-hidden shadow sm:rounded-sm text-lg p-6 mt-8
    }
    div.block {
      background-color: white;
    }
    div.block-3 {
      @apply flex

    }
    div.block-3 div.block {
      flex: 1 1 30%;
    }
    div.block-3 .block:first-child {
      margin-right:  10px;
    }
    div.block-3 .block:last-child {
      margin-left:  10px;
    }

  </style>

<template>
<div id="page">
  <div class="relative flex items-top justify-center min-h-screen bg-pink-100 bg-a100c-1 sm:items-center sm:pt-0">
    <div class="max-w-4xl mx-auto sm:px-6 lg:px-12">
      <div class="flex">
        <div class="flex align-center justify-center mt-8 pt-8 pl-10 sm:pt-0 mr-auto">
          <img src="~/assets/a-thousand-channels--logo-variant-a--short.png" title="A thousand channels">
        </div>
        <div class="flex justify-right ml-auto mt-auto px-2">

         <nuxt-link
            v-for="locale in $i18n.locales"
            :key="locale.code"
            :to="switchLocalePath(locale.code)"
            class="text-link mr-2 px-1">
            {{ locale.code }}
          </nuxt-link>

        </div>
      </div>

      <div class="mt-8 bg-white overflow-hidden shadow sm:rounded-smX p-6">
        <h1 class="leading-7">
          A Thousand Channels –  {{ $t('project_part1') }} <img src="~/assets/lgbtq+_rainbow_flag_quasar_progress_flag_variant.svg" class="h-7 inline p-1" title="Pride flag variant based on Daniel Quasar's 2018 design combining elements of the Philadelphia flag and the trans pride flag, and brown and black." alt="Pride flag variant based on Daniel Quasar's 2018 design combining elements of the Philadelphia flag and the trans pride flag, and brown and black."> {{ $t('project_part2') }}
        </h1>
      </div>
      <div v-if="$i18n.locale == 'en'">

        <nuxt-content :document="index_en" />

        <div class="block">
          <p class="mt-3 text-gray-800">
             Are you interested in collaboration and exchange about coding and design in queer contexts? Or do you have a little time for code reviews, translations and acceptance testing? We welcome your support and feedback :)
          </p>
          <p class="mt-3 text-gray-600">
            <em>A thousand channels</em> is supported by the Prototype Fund :)
          </p>
          <p class="mt-3 text-gray-600">
            Please <a href="https://github.com/a-thousand-channels/" class="text-link" target="_blank">visit us at Github</a> or send us an e-mail at
            <a href="mailto:hello@a-thousand-channels.xyz" class="text-link">
            hello@a-thousand-channels.xyz 📪
            </a>
          </p>
        </div>
      </div>
      <div v-if="$i18n.locale == 'de'" class="">

        <nuxt-content :document="index_de" />



        <div class="mt-3 text-gray-600 overflow-hidden p-6">
          <h3 class="mb-6">Showcase</h3>
          <div class="mx-4 px-8 py-4 bg-slate-200 bg-white ">
            <img src="https://via.placeholder.com/600x200" class="p-4">
            <h4>Intersections & Constellations. From Gay to Queer</h4>
            <p>
               Aktuell arbeitet die Working group „Queer narratives, mapped“ an einer Karte, die mit dem zeitlichen Schwerpunkt in den 90er Jahren und dem räumlichen Fokus auf Bremen erzählt, wie sich aus lesbischen und schwulen Nischen queere Kulturen und Bündnisse entwickelt haben.
               Aus Interviews und der Sammlung von Flyern, Postern, Fotos und anderen Druckerzeugnissen entsteht eine Karte, die von unterschiedlichen, teils persönlichen Perspektiven auf die Entstehung von queeren Communities und Koalitionen erzählt.
               <em>Work in Progress</em>
            </p>
          </div>
        </div>
        <div class="mt-3 text-gray-600 bg-white overflow-hidden shadow sm:rounded-smX p-6">
          <p>
            Besucht uns <a href="https://github.com/a-thousand-channels/" class="text-link">bei Github</a> oder sendet uns eine E-Mail an
            <a href="mailto:hello@a-thousand-channels.xyz" class="text-link">
            hello@a-thousand-channels.xyz 📪
            </a>
          </p>
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
      index_es: []

    }
  },
  async fetch() {
    this.index_de = await this.$content('index_de', { deep: true }).fetch()
    this.index_en = await this.$content('index_en', { deep: true }).fetch()
  }

}

</script>