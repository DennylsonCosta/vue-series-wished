<template>
<div class="conteiner-fluid">
  <h1>Watchlist</h1>
  <div class="row">
    <div
      class="col-3"
      :key="item.id"
      v-for="item in watchlist"
    >
      <serie-box :serie="item" />
    </div>
  </div>
</div>
</template>

<script>
import { mapActions, mapState } from 'vuex'
import SerieBox from '@/components/SerieBox'

export default {
  components: {
    SerieBox
  },
  mounted() {
    this.ActionFindWatchlist()
  },
  computed: {
    ...mapState('watchlist', ['watchlist'])
  },
  methods: {
    ...mapActions('watchlist', ['ActionFindWatchlist'])
  }
}
</script>

<style>

</style>
