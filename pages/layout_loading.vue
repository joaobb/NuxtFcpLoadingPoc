<template>
  <div>
    <PageContent />
  </div>
</template>

<script>
import PageContent from '../components/PageContent'

export default {
  name: 'LoadingLayoutPage',
  components: {
    PageContent,
  },
  layout: 'loaded',
}
</script>
