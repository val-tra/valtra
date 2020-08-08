<template>
  <div
    class="navbar-item has-dropdown"
    :class="{ 'is-active': results.length }"
  >
    <div
      class="control has-icons-left"
      :class="{ 'is-loading': loading }"
    >
      <input
        v-model="query"
        class="input"
        type="search"
        autocomplete="off"
        placeholder="Recherche"
        @keyup.esc="clear"
      >
      <span class="icon is-small is-left">
        <i class="fas fa-search" />
      </span>
    </div>

    <div
      v-if="results.length"
      class="navbar-dropdown is-right"
    >
      <nuxt-link
        v-for="result in results"
        :key="result.slug"
        class="navbar-item"
        :to="result.path"
        @click.native="clear"
      >
        {{ result.title }}
      </nuxt-link>
    </div>
  </div>
</template>

<script>
export default {
  data () {
    return {
      query: '',
      results: [],
      loading: false
    }
  },
  watch: {
    async query (query) {
      if (!query) {
        this.results = []
        this.loading = false
        return
      }

      // Perform search if there is some text in the query property
      this.loading = true
      this.results = await this.$content('', { deep: true })
        .sortBy('createdAt', 'asc')
        .limit(12)
        .search(query)
        .fetch()
      this.loading = false
    }
  },
  methods: {
    clear () {
      // console.log('CLEAR')
      this.results = []
      this.query = ''
      this.loading = false
    }
  }
}
</script>
