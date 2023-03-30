<template>
  <div>
    <PageContent />
  </div>
</template>

<script>
import PageContent from '../components/PageContent'

export default {
  name: 'LoadingPage',
  components: {
    PageContent,
  },

  mounted() {
    this.$nextTick(() => {
      console.log(this.$nuxt.$loading.start)
      this.$nuxt.$loading.start()

      setTimeout(() => {
        this.$nuxt.$loading.finish?.()
      }, 2000)
    })
  },
}
</script>
