<template>
  <div id="homepage-layout">
    <!-- MAIN NAV -->
    <app-navigation />
    <!-- MAIN CONTENT -->
    <Nuxt />
    <!-- FOOTER -->
    <app-footer />
  </div>
</template>

<script>
import AppFooter from '@/components/app-footer.vue'
import AppNavigation from '@/components/app-navigation.vue'

export default {
  components: { AppFooter, AppNavigation }
}
</script>
