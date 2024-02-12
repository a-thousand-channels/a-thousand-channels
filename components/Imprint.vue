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
      @apply pb-0 pt-1 pl-5 pr-5 text-xl
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
          <nuxt-link to="/">
            <img src="~/assets/a-thousand-channels--logo-variant-a--short.png" title="A thousand channels">
          </nuxt-link>
        </div>
        <div class="flex justify-right ml-auto mt-auto px-2">

        </div>
      </div>
      <div class="mt-8 bg-white overflow-hidden shadow sm:rounded-md p-6">
        <h1 class="leading-7">
          <nuxt-link to="/">
            A  Thousand Channels –  {{ $t('project_part1') }} <img src="~/assets/lgbtq+_rainbow_flag_quasar_progress_flag_variant.svg" class="h-6 inline p-1" title="Pride flag variant based on Daniel Quasar's 2018 design combining elements of the Philadelphia flag and the trans pride flag, and brown and black." alt="Pride flag variant based on Daniel Quasar's 2018 design combining elements of the Philadelphia flag and the trans pride flag, and brown and black."> {{ $t('project_part2') }}
          </nuxt-link>
        </h1>
      </div>

      <div class="mt-4 bg-white overflow-hidden shadow sm:rounded-md text-sm p-6">
        <h3 class="text-semibold">Credits</h3>
        <p>Illustration by <a href="https://www.instagram.com/btch_delabutch/" class="text-link">Pau*Schwer</a> // Digital Art Work by <a href="https://www.instagram.com/daphne.jaramillo/" class="text-link">D. Jaramillo</a></p>
        <p>Stopmotion video by <a href="https://www.instagram.com/garabatos.atelier/" class="text-link">Garabatos Atelier</a> </p>
      </div>
      <div class="mt-4 bg-white overflow-hidden shadow sm:rounded-md text-sm p-6">
        <h3 class="text-semibold">Impressum</h3>
        <p class="text-gray-800">
          Angaben gemäß § 5 TMG
        </p>
        <p class="text-gray-800">
          <span class="font-semibold">A 1000 Channels. Ein Projekt von Thomas Böker, Dafne Jaramillo und Ulf Treger</span><br />
          E-Mail: <a href="mailto:hello@a-thousand-channels.xyz" class="text-link">hello@a-thousand-channels.xyz</a><br/>
          Postanschrift: A Thousand Channels, Gaußstraße 25b, D-22765 Hamburg<br />
        </p>
        <p>
          Siehe auch unsere Erklärung zum <nuxt-link to="/privacy" class="text-link">Datenschutz</nuxt-link>
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
