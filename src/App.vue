<template>
  <div id="app">
    <SiteHead/>
    <SiteMain/>
    <SiteFoot/>
  </div>
</template>

<script>
import SiteHead from '@/components/HeadComponent.vue'
import SiteMain from '@/components/MainComponent.vue'
import SiteFoot from '@/components/FootComponent.vue'

export default {
  name: 'App',
  components: {
    SiteHead,
    SiteMain,
    SiteFoot
  }
}
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Source+Sans+Pro&display=swap');
</style>
