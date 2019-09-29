<template>
  <div>

    <section>



    </section>
    
  </div>

</template>

<script>
import playlistsQuery from '~/apollo/queries/playlists'

export default {
  data() {
    return {
      // Initialize an empty restaurants variabkle
      playlists: [],
      query: ''
    }
  },
  apollo: {
    playlists: {
      prefetch: true,
      query: playlistsQuery
    }
  }
}
</script>
