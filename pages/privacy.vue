<template>
  <Privacy />
</template>

<script>
export default {
 data() {
    return {
      title: 'Datenschutz  – A thousand channels'
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
  },
  methods: {
  }
}
</script>
