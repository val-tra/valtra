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
            Scouts confesionnels au vallon
          </h2>
        </div>
      </div>
    </section>
    <!-- Content for homepage -->
    <section class="section">
      <div class="container">
        <div class="columns">
          <div class="column">
            <nuxt-content :document="page" />
          </div>
          <div class="column is-4">
            <h1 class="title">
              Prochaines activités
            </h1>
            <up-next />
          </div>
        </div>
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
