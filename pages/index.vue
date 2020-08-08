<template>
  <div id="home-page">
    <!-- Homepage header -->
    <section class="hero is-medium is-primary has-home-background-image">
      <div class="hero-body">
        <div class="container">
          <h1 class="title">
            Flambeaux du Val-de-travers
          </h1>
          <h2 class="subtitle">
            Aventure - Amitiés - Nature
          </h2>
        </div>
      </div>
    </section>
    <!-- Content for homepage -->
    <section class="section">
      <div class="container">
        <nuxt-content :document="page" />
      </div>
    </section>
  </div>
</template>

<script>
export default {
  layout: 'home',
  async asyncData ({ $content }) {
    const page = await $content('home').fetch()

    return {
      page
    }
  }
}
</script>
