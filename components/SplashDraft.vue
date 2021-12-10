<style>
   .bg-a100c-1 {
      background: rgb(255,0,249);
      background: linear-gradient(90deg, rgba(255,0,249,0.15) 0%, rgba(255,117,0,0.15) 50%, rgba(255,0,35,0.15) 100%);
   }
   .bg-a100c-2 {
      background: rgb(255,0,249);
      background: linear-gradient(90deg, rgba(255,117,0,0.15) 0%, rgba(255,0,35,0.15) 50%, rgba(255,0,249,0.15) 100% );
   }
   .bg-a100c-3 {
      background: rgb(255,0,249);
      background: linear-gradient(90deg, rgba(255,0,35,0.15) 0%, rgba(255,0,249,0.15) 50%, rgba(255,117,0,0.15) 100% );
   }
    button.text-link,
    a.text-link {
      text-decoration: none;
      background-image: linear-gradient(120deg, #fde68a 0, #fde68a 100%);
      background-repeat: no-repeat;
      background-size: 100% 0.4em;
      background-position: 0 100%;
    }
</style>

<template>
<div id="page">
  <div class="relative flex items-top justify-center min-h-screen bg-pink-100 bg-a100c-1 sm:items-center sm:pt-0">
    <link href="https://cdn.jsdelivr.net/npm/tailwindcss@2.1.2/dist/tailwind.min.css" rel="stylesheet">
    <div class="max-w-4xl mx-auto sm:px-6 lg:px-12">
      <div class="flex">
        <div class="flex align-center justify-center mt-8 pt-8 sm:pt-0 mr-auto">
          <img src="a-thousand-channels--logo-variant-a--short.png" title="A thousand channels">
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
      <div class="mt-8 bg-white overflow-hidden shadow sm:rounded-lg p-6">
        <h2 class="text-2xl leading-7 font-semibold">
          A Thousand Channels –  {{ $t('project') }}
        </h2>
      </div>
      <div v-if="$i18n.locale == 'en'" class="mt-8 bg-white overflow-hidden shadow sm:rounded-lg p-6">
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
          Please <a href="https://github.com/a-thousand-channels/" class="text-link">visit us at Github</a> or send us an e-mail at
          <a href="mailto:hello@a-thousand-channels.xyz" class="text-link">
          hello@a-thousand-channels.xyz 📪
          </a>
        </p>
      </div>
      <div v-if="$i18n.locale == 'de'" class="">
        <p class="mt-3 text-gray-800 mt-8 bg-white overflow-hidden shadow sm:rounded-lg p-6">
              "A thousand channels" ist ein Softwareprojekt. Wir entwicklen seit September 2021 eine queere Mappingplattform. Wir wollen damit eine leicht zugängliche Möglichkeit schaffen, eigene queere Narrationen auf einer Karte zu visualisieren und zu veröffentlichen.
               Die vielfältigen sozialen und politischen Aktivitäten queerer Menschen sind meist flüchtig, temporär und kein selbstverständlicher Teil des öffentlichen Bildes einer Stadt. Wir wollen eine Plattform entwickeln, um queeren Akteur*innen und Gruppen eine Möglichkeit zu bieten, von diesen Räumen und Ereignissen zu berichten.
        </p>
        <p class="mt-3 text-gray-800 mt-8 bg-white overflow-hidden shadow sm:rounded-lg p-6">
          <b>Mitmachen</b>
          <br>
               Ihr möchtet queere Geschichten erzählen und kartieren? Ausgehend von Orten, Events, Gruppen, Aktionen oder auch Menschen?<br>
               Mit „A 1000 channels“ wollen wir Euch eine Möglichkeit bieten, queere Geschichte(n) zu erzählen und zu dokumentieren. Dies können die queere Kneipenkultur in einer bestimmten Stadt oder während einer bestimmten Zeit sein, Aktionen, Interventionen, Demonstrationen einer politischen Bewegung oder auch persönlicher Geschichten, Erlebnisse eines oder mehrerer Menschen sein. Oder auch die Sichtbarmachung von imaginären Orten und spekulativen Zukünften, wie wir uns unser queeres Leben vorstellen.
        </p>
        <p class="mt-3 text-gray-600 mt-8 bg-white overflow-hidden shadow sm:rounded-lg p-6">
          <b>Ein Baukasten</b>
          <br>
             Mit der Plattform „A 1000 channels“ stellen wir einen Baukasten zur Verfügung, mit dem Ihr verschiedene Inhalte und Medien zusammentragen, kombinieren und untereinander, räumlich und zeitlich in Bezug setzen könnt.
             Durch Klick auf eine weltweite Karte, könnt Ihr Orte oder Ereignisse anlegen. Textfelder, der Upload von Bildern, von Audio oder Video  geben Euch verschiedene Möglichkeiten, wie Ihr von den Orten, Ereignissen und den Menschen, die diese erschaffen, erzählen wollt.
             Wir werden bei dem Design der Tools besondere Rücksicht auf den Datenschutz nehmen, Bilder werden automatisch von Metadaten befreit, wir experimentieren mit einer Rasterung von Fotos zur Untkenntlichmachung von Gesichtern und es soll eine Funktion geben, genaue Ortsangaben zu verschleiern.
             Am Ende eines jeden Projektes soll die Idee einer „Map to go“ stehen, eine Karte zum Mitnehmen. Damit wollen wir eine dauerhafte Abhängigkeit von unserer Platform (und unserem Projekt) auflösen. Ihr könnt ihr Eure Karte einfach mitnehmen und auf Eurer Website, Eurem eigenen Server veröffentlichen, ohne dass ihr dafür Software installieren müßt.
        </p>
        </p>
        <p class="mt-3 text-gray-600 mt-8 bg-white overflow-hidden shadow sm:rounded-lg p-6">
          <b>Feedback</b>
          <br>
             Wenn Ihr eine Idee für queere Mappings habt, meldet Euch gerne bei uns.<br>
             Aktuell suchen wir für Januar und Februar 2022 noch Menschen mit Ideen für Mappings, die das, woran wir gerade arbeiten, in der Praxis ausprobieren.<br>
             Ihr habt Interesse an Kollaboration und Austausch über Coding und Design in queeren Kontexten? Oder ein wenig Zeit für Code Reviews, Übersetzungen und Akzeptanz Testing? Wir freuen uns über Unterstützung :)<br>
             Euer Feedback hilft uns, die Software zu verbessern
        </p>
        <p class="mt-3 text-gray-600 mt-8 bg-white overflow-hidden shadow sm:rounded-lg p-6">
          <b>Showcase</b>
        <br>
         <b>Intersections & Constellations. From Gay to Queer</b>
        <br>
             Aktuell arbeitet die Working group „Queer narratives, mapped“ an einer Karte, die mit dem zeitlichen Schwerpunkt in den 90er Jahren und dem räumlichen Fokus auf Bremen erzählt, wie sich aus lesbischen und schwulen Nischen queere Kulturen und Bündnisse entwickelt haben.
             Aus Interviews und der Sammlung von Flyern, Postern, Fotos und anderen Druckerzeugnissen entsteht eine Karte, die von unterschiedlichen, teils persönlichen Perspektiven auf die Entstehung von queeren Communities und Koalitionen erzählt.
             <em>Work in Progress</em>
        </p>
        <p class="mt-3 text-gray-600 mt-8 bg-white overflow-hidden shadow sm:rounded-lg p-6">
          Besucht uns <a href="https://github.com/a-thousand-channels/" class="text-link">bei Github</a> oder sendet uns eine E-Mail an
          <a href="mailto:hello@a-thousand-channels.xyz" class="text-link">
          hello@a-thousand-channels.xyz 📪
          </a>
        </p>

      </div>

      <div v-if="$i18n.locale == 'es'" class="mt-8 bg-white overflow-hidden shadow sm:rounded-lg p-6">
        <p class="mt-3 text-gray-800">
          <strong>{{ $t('hello') }}</strong>
        </p>
        <p class="mt-3 text-gray-800">
          <em>... Texto siguiente ...</em>
        </p>

      </div>
      <div class="flex justify-center p-4 m-2 mb-8 space-x-2">
        <a href="https://www.a-thousand-channels.xyz/" target="_blank" class="text-link">
          A Thousand Channels – a queer 🏳️‍🌈 mapping 🗺 platform 🎁
        </a>
      </div>

    </div>
  </div>
</div>
</template>
