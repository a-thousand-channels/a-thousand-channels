<template>
  <div class="p-4 m-2 pl-8 pr-4 mb-8">
    <div class="flex">
      <div class="flex mr-auto">
          <button @click="scrollToTop"><svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" width="20" height="20"><path fill="none" d="M0 0h24v24H0z"/><path d="M12 10.828l-4.95 4.95-1.414-1.414L12 8l6.364 6.364-1.414 1.414z"/></svg> To top</button>

      </div>
      <div class="flex justify-right ml-auto mt-auto">
         <nuxt-link
            v-for="locale in $i18n.locales"
            v-if="locale.active == true"
            :key="locale.code"
            :to="switchLocalePath(locale.code)"
            class="text-link2 mr-2 px-1 pb-1 text-black">
            {{ locale.code }}
          </nuxt-link>
      </div>
    </div>
    <div class="pt-2 pb-2">

        <a href="https://www.a-thousand-channels.xyz/" target="_blank" class="text-link">
          A Thousand Channels – a queer <img src="~/assets/lgbtq+_rainbow_flag_quasar_progress_flag_variant.svg" class="h-4 inline p-0.5" title="Pride flag variant based on Daniel Quasar's 2018 design combining elements of the Philadelphia flag and the trans pride flag, and brown and black." alt="Pride flag variant based on Daniel Quasar's 2018 design combining elements of the Philadelphia flag and the trans pride flag, and brown and black."> mapping 🌎 platform 🎁
        </a>

    </div>
    <hr />
    <div class="pt-2 pb-2 text-sm">
      <div v-if="$i18n.locale == 'de'">
        <p class="p-0">
          Gefördert vom <a href="https://www.bmbf.de/" class="text-link" target="_blank" >Bundesministerium für Bildung und Forschung</a> von 9'2021 – 2'2022 <span class="text-gray-800">(Förderkennzeichen 01IS21S54)</span> und unterstützt vom <a href="https://prototypefund.de/" class="text-link" target="_blank">Protoype Fund</a>
        </p>
        <p class="p-0">
          <a href="https://www.bmbf.de/" target="_blank">
            <img src="/BMBF_Logo.svg" class="h-40 inline-block pr-16" alt="Logo des Bundesministeriums für Bildung und Forschung">
          </a>
          <a href="https://prototypefund.de/" target="_blank">
            <img src="/PrototypeFund_Logo.svg" class="h-28 inline-block" alt="Logo des Prototype Funds">
          </a>
        </p>
      </div>
      <div v-else>
        <p class="p-0">
          Funded by <a href="https://www.bmbf.de/bmbf/en/home/home_node.html" class="text-link" target="_blank" >Federal Ministry of Education and Research</a> <span class="text-gray-800">(9'2021 – 2'2022, funding code 01IS21S54)</span> and supported by <a href="https://prototypefund.de/" class="text-link" target="_blank">Prototype Fund</a>
        </p>
        <p class="p-0">
          <a href="https://www.bmbf.de/bmbf/en/home/home_node.html" target="_blank">
            <img src="BMBF_Logo.svg" class="h-40 inline-block pr-16" alt="Logo of the Federal Ministry of Educatio and Research">
          </a>
          <a href="https://prototypefund.de/" target="_blank">
            <img src="PrototypeFund_Logo.svg" class="h-28 inline-block" alt="Logo of Prototype Fund">
          </a>
        </p>
      </div>
    </div>
    <div class="pt-2 pb-2 text-sm">
      A Thousand Channels 2021/22 – <nuxt-link to="/imprint" class="text-link">Impressum</nuxt-link> – <nuxt-link to="/privacy" class="text-link">Datenschutz</nuxt-link>
    </div>
    <hr />
  </div>
</template>

<script>
export default {
 data() {
    return {

    }
  },
  methods: {
    scrollToTop() {
      window.scrollTo({ top: 0, behavior: 'smooth' })
    }
  }
}
</script>
