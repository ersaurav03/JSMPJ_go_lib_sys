<template>
  <div>
    <section class="hero is-info is-fullheight">
      <!-- Hero head: will stick at the top -->
      <div class="hero-head">
        <nav class="navbar is-info">
          <div class="navbar-brand">
            <a class="navbar-item" href="#">
              <img
                src="../../public/logo.svg"
                alt="Bulma: a modern CSS framework based on Flexbox"
                width="112"
                height="28"
              />
            </a>
            <div
              class="navbar-burger burger"
              @click="showNav =! showNav"
              data-target="navbarExampleTransparentExample"
            >
              <span></span>
              <span></span>
              <span></span>
            </div>
          </div>

          <div
            id="navbarExampleTransparentExample"
            class="navbar-menu"
            :class="{'is-active':showNav}"
          >
            <div class="navbar-start">
              <a class="navbar-item" href="#">
                <router-link to class="has-text-dark">Home</router-link>
              </a>
              <a class="navbar-item" href="#">
                <router-link to="#" class="has-text-dark">Search</router-link>
              </a>
              <a class="navbar-item" href="#">
                <router-link to="#" class="has-text-dark">Add Comments</router-link>
              </a>
            </div>

            <div class="navbar-end">
              <div class="navbar-item">
                <div class="field is-grouped">
                  <p class="control">
                    <strong>Welcome user:- User Name</strong>
                    <span class="icon is-large">
                      <i class="fas fa-user black"></i>
                    </span>
                  </p>
                  <p class="control">
                    <span class="icon is-large">
                      <a class="button is-dark is-outlined">
                        <i class="fas fa-sign-out-alt">Logout</i>
                      </a>
                    </span>
                  </p>
                </div>
              </div>
              <div class="navbar-item">
                <div class="field is-grouped">
                  <p class="control"></p>
                </div>
              </div>
            </div>
          </div>
        </nav>
      </div>

      <!-- Hero content: will be in the middle -->
      <div class="hero-body">
        <div class="container has-text-centered">
          <div class="tile is-ancestor">
            <div class="tile is-4 is-vertical is-parent">
              <div class="tile is-child box">
                <p class="title has-text-dark">User Detail</p>
                <article class="media">
                  <figure class="media-left">
                    <p class="image is-64x64">
                      <i class="fas fa-user fa-4x"></i>
                    </p>
                  </figure>
                  <div class="media-content">
                    <div class="content">
                      <p>
                        <strong>Name :-</strong>
                        <small>Saurav Kumar</small>
                        <br />
                        <strong>Email :-</strong>
                        <small>er.saurav03@gmail.com</small>
                        <br />
                        <strong>Phone Number :-</strong>
                        <small>9988776655</small>
                        <br />
                      </p>
                    </div>
                  </div>
                </article>
              </div>
            </div>
            <div class="tile is-parent">
              <div class="tile is-child box">
                <p class="title has-text-dark">Three</p>
                <b-field>
                  <p class="control">
                    <b-dropdown>
                      <button class="button" slot="trigger">
                        <span>Book Type</span>
                        <b-icon icon="menu-down"></b-icon>
                      </button>

                      <b-dropdown-item value="open_issues">TextBook</b-dropdown-item>
                      <b-dropdown-item value="your_issues">CookBook</b-dropdown-item>
                      <b-dropdown-item value="pull_requests">Anthology</b-dropdown-item>
                      <b-dropdown-item value="everything">Graphic</b-dropdown-item>
                    </b-dropdown>
                  </p>
                  <b-input icon="magnify" type="search" placeholder="Search..." expanded></b-input>
                </b-field>
              </div>
            </div>
          </div>
        </div>
      </div>

      <!-- Hero footer: will stick at the bottom -->
      <div class="hero-foot">
        <nav class="tabs">
          <div class="container">
            <ul>
              <li class="is-active">
                <a>Overview</a>
              </li>
              <li>
                <a>Books</a>
              </li>
              <li>
                <a>Journals</a>
              </li>
              <li>
                <a>Novels</a>
              </li>
              <li>
                <a>Timings</a>
              </li>
              <li>
                <a>Layout</a>
              </li>
            </ul>
          </div>
        </nav>
      </div>
    </section>
  </div>
</template>
<script>
export default {
  data() {
    return {
      showNav: false
    };
  }
};
</script>


