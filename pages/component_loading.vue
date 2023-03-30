<template>
  <div>
    <CustomLoadingBar />

    <PageContent />
  </div>
</template>

<script>
import PageContent from '../components/PageContent'
import CustomLoadingBar from '../components/CustomLoadingBar'

export default {
  name: 'CustomLoadingPage',
  components: {
    PageContent,
    CustomLoadingBar,
  },
}
</script>
