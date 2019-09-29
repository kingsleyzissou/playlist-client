<template>
  <div class="container">
    <section class="columns" style="padding: 1em">
      <div class="column is-12">
        <div class="card" v-for="(playlist, index) in playlists" :key="index">
          <div class="card-content">
            <p class="title">{{ playlist.name }}</p>
            <p class="heading">{{ playlist.songs.length }} songs</p>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
import playlistsQuery from "~/apollo/queries/playlists";

export default {
  data() {
    return {
      // Initialize an empty restaurants variabkle
      playlists: [],
      query: ""
    };
  },
  apollo: {
    playlists: {
      prefetch: true,
      query: playlistsQuery
    }
  }
};
</script>
