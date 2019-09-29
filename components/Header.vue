<template>
  <div>
    <!-- Hero head: will stick at the top -->
    <div class="hero-head">
      <nav class="navbar main-navbar">
        <div class="container">
          <div class="navbar-brand">
            <a href="/" class="navbar-item">
              <figure class="image is-24x24">
                <img src="/images/logo.png" alt="Placeholder image" />
              </figure>&nbsp;&nbsp;
              WEBMARK.IO
            </a>
            <span class="navbar-burger burger">
              <span></span>
              <span></span>
              <span></span>
            </span>
          </div>
          <div class="navbar-menu">
            <div class="navbar-end">
              <a href="/dashboard" class="navbar-item">Dashboard</a>
              <a href="/about" class="navbar-item">About</a>

              <!---->
            </div>
          </div>
        </div>
      </nav>
    </div>
  </div>
</template>

<style>
  .main-navbar {
    padding: 20px 0;
  }
</style>