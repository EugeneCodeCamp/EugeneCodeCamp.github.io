<template>
  <b-navbar toggleable="md" type="dark" class="navbar">
    <b-navbar-brand href="#">ECC</b-navbar-brand>
    <b-navbar-toggle target="nav-collapse" />
    <b-collapse id="nav-collapse" is-nav>
      <b-navbar-nav class="ml-auto">
        <b-nav-item href="#about">About</b-nav-item>
        <b-nav-item href="#events">Events</b-nav-item>
        <b-nav-item href="#resources">Resources</b-nav-item>
      </b-navbar-nav>
    </b-collapse>
  </b-navbar>
</template>

<script>
export default {}
</script>

<style scoped>
.navbar {
  padding-top: 1rem;
  padding-bottom: 1rem;
  font-family: 'Montserrat', -apple-system, BlinkMacSystemFont, 'Segoe UI',
    Roboto, 'Helvetica Neue', Arial, 'Noto Sans', sans-serif,
    'Apple Color Emoji', 'Segoe UI Emoji', 'Segoe UI Symbol', 'Noto Color Emoji';
  font-weight: 700;
  background-color: #35495e;
}

.navbar .navbar-brand {
  color: #fff;
}

.navbar .navbar-nav {
  margin-top: 1rem;
}

.navbar .navbar-nav li.nav-item a.nav-link {
  color: #fff;
}

.navbar .navbar-nav li.nav-item a.nav-link:hover {
  color: #1abc9c;
}

.navbar .navbar-nav li.nav-item a.nav-link:active,
.navbar .navbar-nav li.nav-item a.nav-link:focus {
  color: #fff;
}

.navbar .navbar-nav li.nav-item a.nav-link.active {
  color: #1abc9c;
}

.navbar .navbar-toggler {
  font-size: 80%;
  padding: 0.8rem;
}

@media (min-width: 992px) {
  .navbar {
    padding-top: 1.5rem;
    padding-bottom: 1.5rem;
    transition: padding-top 0.3s, padding-bottom 0.3s;
  }
  .navbar .navbar-brand {
    font-size: 1.75em;
    transition: font-size 0.3s;
  }
  .navbar .navbar-nav {
    margin-top: 0;
  }
  .navbar .navbar-nav > li.nav-item > a.nav-link.active {
    color: #fff;
    background: #1abc9c;
  }
  .navbar .navbar-nav > li.nav-item > a.nav-link.active:active,
  .navbar .navbar-nav > li.nav-item > a.nav-link.active:focus,
  .navbar .navbar-nav > li.nav-item > a.nav-link.active:hover {
    color: #fff;
    background: #1abc9c;
  }
  .navbar.navbar-shrink {
    padding-top: 0.5rem;
    padding-bottom: 0.5rem;
  }
  .navbar.navbar-shrink .navbar-brand {
    font-size: 1.5em;
  }
}
</style>
