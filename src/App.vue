<template>
  <div id="app">
    <SiteHead/>
    <SiteMain/>
  </div>
</template>

<script>
import SiteHead from '@/components/HeadComponent.vue'
import SiteMain from '@/components/MainComponent.vue'

export default {
  name: 'App',
  components: {
    SiteHead,
    SiteMain
  }
}
</script>

<style lang="scss">

</style>
