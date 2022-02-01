<template>
  <div class="p-4 m-2 pl-8 pr-4 mb-8">
    <div class="text-left">
        <button @click="scrollToTop"><svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" width="20" height="20"><path fill="none" d="M0 0h24v24H0z"/><path d="M12 10.828l-4.95 4.95-1.414-1.414L12 8l6.364 6.364-1.414 1.414z"/></svg></button>
    </div>
    <div class="pt-2 pb-2">
      <a href="https://www.a-thousand-channels.xyz/" target="_blank" class="text-link">
        A Thousand Channels – a queer <img src="~/assets/lgbtq+_rainbow_flag_quasar_progress_flag_variant.svg" class="h-4 inline p-0.5" title="Pride flag variant based on Daniel Quasar's 2018 design combining elements of the Philadelphia flag and the trans pride flag, and brown and black." alt="Pride flag variant based on Daniel Quasar's 2018 design combining elements of the Philadelphia flag and the trans pride flag, and brown and black."> mapping 🗺 platform 🎁
      </a>
    </div>
    <div class="pt-2 pb-2 text-sm">
      <div v-if="$i18n.locale == 'de'">
        <p>
          Gefördert vom <a href="https://www.bmbf.de/" class="text-link" target="_blank" >Bundesministerium für Bildung und Forschung</a> und unterstützt vom <a href="https://prototypefund.de/" class="text-link" target="_blank">Prototype Fund</a>
        </p>
        <p>
          <a href="https://www.bmbf.de/" target="_blank">
            <img src="BMBF_Logo.svg" class="h-40 inline-block pr-8" alt="Logo des Bundesministeriums">
          </a>
          <a href="https://prototypefund.de/" target="_blank">
            <img src="PrototypeFund_Logo.svg" class="h-32 inline-block" alt="Logo des Prototype Funds">
          </a>
        </p>
      </div>
      <div v-else>
        <p>
          Funded by <a href="https://www.bmbf.de/bmbf/en/home/home_node.html" class="text-link" target="_blank" >Federal Ministry of Education and Research</a> and supported by <a href="https://prototypefund.de/" class="text-link" target="_blank">Prototype Fund</a>
        </p>
        <p>
          <a href="https://www.bmbf.de/bmbf/en/home/home_node.html" target="_blank">
            <img src="BMBF_Logo.svg" class="h-40 inline-block pr-8" alt="Logo of the Federal Ministry">
          </a>
          <a href="https://prototypefund.de/" target="_blank">
            <img src="PrototypeFund_Logo.svg" class="h-32 inline-block" alt="Logo of Prototype Fund">
          </a>
        </p>
      </div>
    </div>
    <div class="pt-2 pb-2 text-sm">
      A Thousand Channels 2021/22 – <nuxt-link to="/imprint" class="text-link">Impressum</nuxt-link> – <nuxt-link to="/privacy" class="text-link">Datenschutz</nuxt-link>
    </div>
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
