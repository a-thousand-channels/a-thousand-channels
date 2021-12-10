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
          <a href="mailto:hello@a-thousand-channels.xyz" style="text-decoration: none; background-image: linear-gradient(120deg, #fde68a 0, #fde68a 100%); background-repeat: no-repeat; background-size: 100% 0.4em; background-position: 0 100%">
          hello@a-thousand-channels.xyz 📪
          </a>
        </p>
      </div>
      <div v-if="$i18n.locale == 'de'" class="mt-8 bg-white overflow-hidden shadow sm:rounded-lg p-6">
        <p class="mt-3 text-gray-800">
          <em>A thousand channels</em> ist ein Softwareprojekt, mit dem wir seit September eine queere Mappingplattform entwickeln. Mit einer „Map to go“ möchten wir eine einfache Möglichkeit anbieten, eigene queere Narrationen geografisch zu visualisieren und zu veröffentlichen.
        </p>
        <p class="mt-3 text-gray-800">
          Habt Ihr Interesse an Kollaboration und Austausch über Coding und Design in queeren Kontexten? Oder ein wenig Zeit für Code Reviews, Übersetzungen und Akzeptanz Testing? Wir freuen uns über Unterstützung und Feedback :)
        </p>
        <p class="mt-3 text-gray-600">
          <em>A thousand channels</em> wird vom Prototype Fund unterstützt :)
        </p>
        <p class="mt-3 text-gray-600">
          Besucht uns <a href="https://github.com/a-thousand-channels/" style="text-decoration: none; background-image: linear-gradient(120deg, #fde68a 0, #fde68a 100%); background-repeat: no-repeat; background-size: 100% 0.4em; background-position: 0 100%">bei Github</a> oder sendet uns eine E-Mail an
          <a href="mailto:hello@a-thousand-channels.xyz" style="text-decoration: none; background-image: linear-gradient(120deg, #fde68a 0, #fde68a 100%); background-repeat: no-repeat; background-size: 100% 0.4em; background-position: 0 100%">
          hello@a-thousand-channels.xyz 📪
          </a>
        </p>

      </div>

      <div v-if="$i18n.locale == 'es'" class="mt-8 bg-white overflow-hidden shadow sm:rounded-lg p-6">
        <p class="mt-3 text-gray-800">
          <strong>{{ $t('hello') }}</strong>

        </p>

      </div>
      <div class="flex justify-center p-4 m-2 mb-8 space-x-2">
        <a href="https://www.a-thousand-channels.xyz/" target="_blank" style="text-decoration: none; background-image: linear-gradient(120deg, #fde68a 0, #fde68a 100%); background-repeat: no-repeat; background-size: 100% 0.4em; background-position: 0 100%">
          A Thousand Channels – a queer 🏳️‍🌈 mapping 🗺 platform 🎁
        </a>
      </div>

    </div>
  </div>
</div>
</template>
