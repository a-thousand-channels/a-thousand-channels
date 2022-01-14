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
      <div class="mt-8 bg-white overflow-hidden shadow sm:rounded-md p-6">
        <h1 class="leading-7">
          A Thousand Channels –  {{ $t('project_part1') }} <img src="~/assets/lgbtq+_rainbow_flag_quasar_progress_flag_variant.svg" class="h-7 inline p-1" title="Pride flag variant based on Daniel Quasar's 2018 design combining elements of the Philadelphia flag and the trans pride flag, and brown and black." alt="Pride flag variant based on Daniel Quasar's 2018 design combining elements of the Philadelphia flag and the trans pride flag, and brown and black."> {{ $t('project_part2') }}
        </h1>
      </div>
      <div v-if="$i18n.locale == 'en'" class="mt-8 bg-white overflow-hidden shadow sm:rounded-md text-lg p-6">
        <p class="mt-3 text-gray-800">
          <strong>{{ $t('hello') }}</strong>
          <em>A thousand channels</em> is a software project with which we are developing a queer mapping portal since September. With a "map to go" we want to offer an easy way to geographically visualise and publish your own queer narratives.
        </p>
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
      <div v-if="$i18n.locale == 'de'" class="">
        <div class="mt-3 text-gray-800 mt-8 bg-white overflow-hidden shadow sm:rounded-md text-lg p-6">
          <p>
              "A thousand channels" ist ein Softwareprojekt. Wir entwicklen seit September 2021 eine queere Mappingplattform. Wir wollen damit eine leicht zugängliche Möglichkeit schaffen, eigene queere Narrationen auf einer Karte zu visualisieren und zu veröffentlichen.
          </p>
          <p>
               Die vielfältigen sozialen und politischen Aktivitäten queerer Menschen sind meist flüchtig, temporär und kein selbstverständlicher Teil des öffentlichen Bildes einer Stadt. Wir wollen eine Plattform entwickeln, um queeren Akteur*innen und Gruppen eine Möglichkeit zu bieten, von diesen Räumen und Ereignissen zu berichten.
          </p>
        </div>
        <div class="mt-3 text-gray-800 mt-8 bg-white overflow-hidden shadow sm:rounded-md text-md p-6">
          <h3>Mitmachen</h3>
          <p>
               Ihr möchtet queere Geschichten erzählen und kartieren? Ausgehend von Orten, Events, Gruppen, Aktionen oder auch Menschen?
          </p>
          <p>
               Mit „A 1000 channels“ wollen wir Euch eine Möglichkeit bieten, queere Geschichte(n) zu erzählen und zu dokumentieren. Dies können die queere Kneipenkultur in einer bestimmten Stadt oder während einer bestimmten Zeit sein, Aktionen, Interventionen, Demonstrationen einer politischen Bewegung oder auch persönlicher Geschichten, Erlebnisse eines oder mehrerer Menschen sein. Oder auch die Sichtbarmachung von imaginären Orten und spekulativen Zukünften, wie wir uns unser queeres Leben vorstellen.
          </p>
        </div>
        <div class="mt-3 text-gray-600 mt-8 bg-white overflow-hidden shadow sm:rounded-md text-md  p-6">
          <h3>Ein Baukasten</h3>
          <p>
             Mit der Plattform „A 1000 channels“ stellen wir einen Baukasten zur Verfügung, mit dem Ihr verschiedene Inhalte und Medien zusammentragen, kombinieren und untereinander, räumlich und zeitlich in Bezug setzen könnt.
          </p>
          <p>
             Durch Klick auf eine weltweite Karte, könnt Ihr Orte oder Ereignisse anlegen. Textfelder, der Upload von Bildern, von Audio oder Video  geben Euch verschiedene Möglichkeiten, wie Ihr von den Orten, Ereignissen und den Menschen, die diese erschaffen, erzählen wollt.
          </p>
          <p>
             Wir werden bei dem Design der Tools besondere Rücksicht auf den Datenschutz nehmen, Bilder werden automatisch von Metadaten befreit, wir experimentieren mit einer Rasterung von Fotos zur Untkenntlichmachung von Gesichtern und es soll eine Funktion geben, genaue Ortsangaben zu verschleiern.
             Am Ende eines jeden Projektes soll die Idee einer „Map to go“ stehen, eine Karte zum Mitnehmen. Damit wollen wir eine dauerhafte Abhängigkeit von unserer Platform (und unserem Projekt) auflösen. Ihr könnt ihr Eure Karte einfach mitnehmen und auf Eurer Website, Eurem eigenen Server veröffentlichen, ohne dass ihr dafür Software installieren müßt.
          </p>
        </div>
        <div class="mt-3 text-gray-600 mt-8 bg-white overflow-hidden shadow sm:rounded-md p-6">
          <h3>Feedback</h3>
          <p>
             Wenn Ihr eine Idee für queere Mappings habt, meldet Euch gerne bei uns.</p>
          <p>
             Aktuell suchen wir für Januar und Februar 2022 noch Menschen mit Ideen für Mappings, die das, woran wir gerade arbeiten, in der Praxis ausprobieren.
          </p>
          <p>
             Ihr habt Interesse an Kollaboration und Austausch über Coding und Design in queeren Kontexten? Oder ein wenig Zeit für Code Reviews, Übersetzungen und Akzeptanz Testing? Wir freuen uns über Unterstützung :)
          </p>
          <p>
             Euer Feedback hilft uns, die Software zu verbessern
          </p>
        </div>
        <div class="mt-3 text-gray-600 mt-8 bg-white overflow-hidden shadow sm:rounded-md p-6">
          <h3>Showcase</h3>

          <h4>Intersections & Constellations. From Gay to Queer</h4>
          <p>
             Aktuell arbeitet die Working group „Queer narratives, mapped“ an einer Karte, die mit dem zeitlichen Schwerpunkt in den 90er Jahren und dem räumlichen Fokus auf Bremen erzählt, wie sich aus lesbischen und schwulen Nischen queere Kulturen und Bündnisse entwickelt haben.
             Aus Interviews und der Sammlung von Flyern, Postern, Fotos und anderen Druckerzeugnissen entsteht eine Karte, die von unterschiedlichen, teils persönlichen Perspektiven auf die Entstehung von queeren Communities und Koalitionen erzählt.
             <em>Work in Progress</em>
          </p>
        </div>
        <div class="mt-3 text-gray-600 mt-8 bg-white overflow-hidden shadow sm:rounded-md p-6">
          <p>
            Besucht uns <a href="https://github.com/a-thousand-channels/" class="text-link">bei Github</a> oder sendet uns eine E-Mail an
            <a href="mailto:hello@a-thousand-channels.xyz" class="text-link">
            hello@a-thousand-channels.xyz 📪
            </a>
          </p>
        </div>

      </div>

      <div v-if="$i18n.locale == 'es'" class="mt-8 bg-white overflow-hidden shadow sm:rounded-md p-6">
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

    }
  }
}
</script>