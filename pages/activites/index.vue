<template>
  <div class="columns">
    <div class="column has-background-white">
      <nuxt-content
        class="content is-medium"
        :document="page"
      />
    </div>
  </div>
</template>

<script>
export default {
  async asyncData ({ $content }) {
    const page = await $content('activites/index').fetch()

    return {
      page
    }
  }
}
</script>
