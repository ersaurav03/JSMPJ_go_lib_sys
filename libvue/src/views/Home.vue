<template>
  <nav class="navbar is-info">
    <div class="navbar-brand">
      <a class="navbar-item" href="#">
        <img
          src="../../public/logo.png"
          alt="Bulma: a modern CSS framework based on Flexbox"
          width="112"
          height="28"
        />
      </a>
      <div class="navbar-burger burger" @click="showNav =! showNav" data-target="navbarExampleTransparentExample">
        <span></span>
        <span></span>
        <span></span>
      </div>
    </div>

    <div id="navbarExampleTransparentExample" class="navbar-menu" :class="{'is-active':showNav}">
      <div class="navbar-start">
        <a class="navbar-item" href="#">Home</a>
        <a class="navbar-item" href="#">About</a>
        <a class="navbar-item" href="#">Contacts</a>
        <a class="navbar-item" href="#">Books</a>

        <div class="navbar-item has-dropdown is-hoverable">
          <a class="navbar-link" href="#">Account</a>
          <div class="navbar-dropdown is-boxed">
            <a class="navbar-item" href="#">Login</a>
            <a class="navbar-item" href="#">SignUp</a>
          </div>
        </div>
      </div>

      <div class="navbar-end">
        <div class="navbar-item">
          <div class="field is-grouped">
            <p class="control">
              <b-field>
                <b-input placeholder="Search..." type="search" icon="magnify"></b-input>
                <p class="control">
                  <button class="button is-info">Search</button>
                </p>
              </b-field>
            </p>
          </div>
        </div>
      </div>
    </div>
  </nav>

  
</template>
<script>
export default {
  data(){
    return{
      showNav:false
    }
  }
}
</script>


