<template>
  <div>
    <section class="hero is-info">
      <!-- Hero head: will stick at the top -->
      <Header></Header>

      <nav class="navbar has-shadow has-text-white" style="background: #3AB6FF">
        <div class="container">
          <!-- <nav class="breadcrumb has-text-white" aria-label="breadcrumbs">
            <ul>
              <li>Dashboard&nbsp;</li>
            </ul>
          </nav> -->
        </div>
      </nav>

    </section>
    <nuxt />
  </div>
</template>

<script>
  import Header from '~/components/Header.vue'

  export default {
    components: {
      Header
    }
  }
</script>
