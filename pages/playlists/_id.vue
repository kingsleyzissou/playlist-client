<template>
  <div class="container">
    <section class="columns" style="padding: 1em">
      <div class="column is-12">
        <div class="card" v-for="(song, index) in playlist.songs" :key="index">
          <div class="card-content">
            <p class="title">{{ song.title }}</p>
            <p class="heading">Artist: {{ song.artist.name }}</p>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
import playlistQuery from "~/apollo/queries/playlist";

export default {
  data() {
    return {
      // Initialize an empty restaurants variabkle
      playlist: {},
      query: ""
    };
  },
  apollo: {
    playlist: {
      prefetch: true,
      query: playlistQuery,
      variables() {
          let id = Number.parseInt(this.$route.params.id);
          return { id };
      }
    }
  }
};
</script>
