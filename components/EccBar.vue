<template>
  <b-navbar toggleable="md" type="dark" class="navbar">
    <b-navbar-brand href="#">ECC</b-navbar-brand>
    <b-navbar-toggle target="nav-collapse" />
    <b-collapse id="nav-collapse" is-nav>
      <b-navbar-nav class="ml-auto">
        <b-nav-item href="#events">EVENTS</b-nav-item>
        <b-nav-item href="#about">ABOUT</b-nav-item>
        <b-nav-item href="#resources">RESOURCES</b-nav-item>
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
  padding-right: 3rem;
  padding-left: 3rem;
  font-family: 'Montserrat', -apple-system, BlinkMacSystemFont, 'Segoe UI',
    Roboto, 'Helvetica Neue', Arial, 'Noto Sans', sans-serif,
    'Apple Color Emoji', 'Segoe UI Emoji', 'Segoe UI Symbol', 'Noto Color Emoji';
  font-weight: 700;
  background-color: #35495e;
}

.navbar .navbar-brand {
  color: #fff;
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

.navbar .nav-item {
  margin-bottom: -0.125rem;
}
.nav-link {
  border: 0.125rem solid transparent;
  border-top-left-radius: 0.8rem;
  border-top-right-radius: 0.8rem;
}
.nav-tabs .nav-link:hover,
.nav-tabs .nav-link:focus {
  border-color: #e9ecef #e9ecef #dee2e6;
}
.nav-tabs .nav-link.disabled {
  color: #6c757d;
  background-color: transparent;
  border-color: transparent;
}
.nav-tabs .nav-link.active,
.nav-tabs .nav-item.show .nav-link {
  color: #495057;
  background-color: #fff;
  border-color: #dee2e6 #dee2e6 #fff;
}
.nav-tabs .dropdown-menu {
  margin-top: -0.125rem;
  border-top-left-radius: 0;
  border-top-right-radius: 0;
}
.nav-pills .nav-link {
  border-radius: 0.5rem;
}
.nav-pills .nav-link.active,
.nav-pills .show > .nav-link {
  color: #fff;
  background-color: #1abc9c;
}
.nav-fill .nav-item {
  flex: 1 1 auto;
  text-align: center;
}
.nav-justified .nav-item {
  flex-basis: 0;
  flex-grow: 1;
  text-align: center;
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
