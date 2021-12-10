<template>
  <SplashDraft />
</template>

<script>
export default {
 data() {
    return {
      title: 'A thousand channels'
    }
  },
  head() {
    return {
      title: this.title,
      meta: [
        {
          hid: 'description',
          name: 'description',
          content: 'My custom description'
        }
      ]
    }
  }
}
</script>
