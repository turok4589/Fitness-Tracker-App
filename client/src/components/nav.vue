<template>
    
    <nav class="navbar container is-fixed-top is-info" role="navigation" aria-label="main navigation">
     <div class="navbar-brand">
    <a class="navbar-item" href="https://bulma.io">
      <img src="../assets/logo.png" height="28">
    </a>

    <a role="button" class="navbar-burger burger" :class="{'is-active': isActive}" @click="isActive = !isActive" aria-label="menu" aria-expanded="false" data-target="navbarBasicExample">
      <span aria-hidden="true"></span>
      <span aria-hidden="true"></span>
      <span aria-hidden="true"></span>
    </a>
  </div>

  <div id="navbarBasicExample" class="navbar-menu" :class="{'is-active': isActive}">

    <div class="navbar-start">
        <router-link to="/"  class="navbar-item" >Home</router-link>
        <router-link to="/about"  class="navbar-item" >About</router-link>

      <div class="navbar-item has-dropdown is-hoverable">
        <a class="navbar-link">
          More
        </a>

        <div class="navbar-dropdown">
          <a class="navbar-item">
            About
          </a>
          <a class="navbar-item">
            Jobs
          </a>
          <a class="navbar-item">
            Contact
          </a>
          <hr class="navbar-divider">
          <a class="navbar-item">
            Report an issue
          </a>
        </div>
      </div>
    </div>

    <div class="navbar-end">
      <div class="navbar-item">
        <div class="buttons">
          <a class="button">
            <strong>Sign up</strong>
          </a>
      <router-link to="/login"  class="button"><strong>Log in</strong></router-link>
        </div>
      </div>
    </div>
  </div>
</nav>
</template>

<script>
export default {
   data: () => ({
       isActive: false
   }), //parantheses tell javascript that the squigglys are the return value
   methods: ({

   })
}

</script>

<style>

</style>