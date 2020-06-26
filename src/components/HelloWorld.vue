<template>
  <div>
    <b-navbar toggleable="lg" type="dark" variant="primary">
    <b-navbar-brand href="#">Home</b-navbar-brand>

    <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

    <b-collapse id="nav-collapse" is-nav>
      <b-navbar-nav>
        <b-nav-item href="#">Blog</b-nav-item>
        <b-nav-item href="#">Services</b-nav-item>
        <b-nav-item href="#">Contact</b-nav-item>
      </b-navbar-nav>
  </div>
</template>

<script>
  export default {
    name: 'HelloWorld',

    data: () => ({
      
    }),
  }
</script>
