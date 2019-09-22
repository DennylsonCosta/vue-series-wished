<template>
<h1>Watchlist</h1>
</template>

<script>
import { mapActions, mapState } from 'vuex'

export default {
  mounted() {
    this.ActionFindWatchlist()
  },
  methods: {
    ...mapActions('watchlist', ['ActionFindWatchlist'])
  }
}
</script>

<style>

</style>
