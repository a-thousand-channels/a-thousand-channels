<template>
  <div>

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
    <img src="/progresiveflagcolor.svg" class="illustration illustration-middle" alt="Pride flag variant based on Daniel Quasar's 2018 design combining elements of the Philadelphia flag and the trans pride flag, and brown and black." title="Pride flag variant based on Daniel Quasar's 2018 design combining elements of the Philadelphia flag and the trans pride flag, and brown and black.">
    <div class="pt-2 pb-2 text-sm">
      A Thousand Channels 2021/2025 – <nuxt-link to="/imprint" class="text-link">Impressum</nuxt-link> – <nuxt-link to="/privacy" class="text-link">Datenschutz</nuxt-link>
    </div>
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
