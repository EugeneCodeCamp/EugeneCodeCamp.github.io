<template>
  <b-navbar
    id="mainNav"
    toggleable="md"
    type="dark"
    class="navbar navbar-expand-lg text-uppercase fixed-top navbar-shrink bg-secondary"
  >
    <div class="container">
      <b-navbar-brand class="navbar-brand" href="#">ECC</b-navbar-brand>
      <b-navbar-toggle target="nav-collapse" />
      <b-collapse id="nav-collapse" is-nav>
        <b-navbar-nav id="navbarResponsive" class="ml-auto">
          <b-nav-item
            class="nav-link py-3 px-0 px-lg-3 rounded text-left"
            href="#events"
            >Events</b-nav-item
          >
          <b-nav-item
            class="nav-link py-3 px-0 px-lg-3 rounded text-left"
            href="#about"
            >About</b-nav-item
          >
          <b-nav-item
            class="nav-link py-3 px-0 px-lg-3 rounded text-left"
            href="#resources"
            >Resources</b-nav-item
          >
        </b-navbar-nav>
      </b-collapse>
    </div>
  </b-navbar>
</template>

<script>
export default {}
</script>

<style></style>
