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
              <a class="navbar-item" href="#">Home</a>
              <a class="navbar-item" href="#">About</a>
              <a class="navbar-item" href="#">Contacts</a>
              <a class="navbar-item" href="#">Books</a>
              <div class="navbar-item has-dropdown is-hoverable">
                <a class="navbar-link" href="#">Account</a>
                <div class="navbar-dropdown is-boxed">
                  <div class="navbar-menu">
                    <div class="navbar-end">
                      <b-dropdown position="is-bottom-right" aria-role="menu">
                        <a class="navbar-item" slot="trigger" role="button">
                          <span class="has-text-dark">
                            <strong>Login</strong>
                            <strong class="is-invisible">hi</strong>
                          </span>
                          <b-icon icon="menu-down"></b-icon>
                        </a>

                        <b-dropdown-item aria-role="menu-item" custom paddingless>
                          <form action>
                            <div class="modal-card" style="width:300px;">
                              <section class="modal-card-body">
                                <b-field label="Email">
                                  <b-input type="email" placeholder="Your email" required></b-input>
                                </b-field>

                                <b-field label="Password">
                                  <b-input
                                    type="password"
                                    password-reveal
                                    placeholder="Your password"
                                    required
                                  ></b-input>
                                </b-field>
                              </section>
                              <footer class="modal-card-foot">
                                <button class="button is-info">Login</button>
                              </footer>
                            </div>
                          </form>
                        </b-dropdown-item>
                      </b-dropdown>
                    </div>
                  </div>
                  <div class="navbar-menu">
                    <div class="navbar-end">
                      <b-dropdown position="is-bottom-right" aria-role="menu">
                        <a class="navbar-item" slot="trigger" role="button">
                          <span class="has-text-dark">
                            <strong>Register</strong>
                          </span>
                          <b-icon icon="menu-down"></b-icon>
                        </a>
                        <b-dropdown-item aria-role="menu-item" custom paddingless>
                          <form action>
                            <div class="modal-card" style="width:300px;">
                              <section class="modal-card-body">
                                <b-field label="Name">
                                  <b-input type="text" placeholder="Enter Your Name" required></b-input>
                                </b-field>
                                <b-field label="Email">
                                  <b-input type="email" placeholder="Your Email Id" required></b-input>
                                </b-field>
                                <b-field label="Phone">
                                  <b-input
                                    type="number"
                                    placeholder="Your Mobile Number Id"
                                    required
                                  ></b-input>
                                </b-field>
                                <b-field label="Password">
                                  <b-input
                                    type="password"
                                    password-reveal
                                    placeholder="Enter Your password"
                                    required
                                  ></b-input>
                                </b-field>
                              </section>
                              <footer class="modal-card-foot">
                                <button class="button is-info">Register</button>
                              </footer>
                            </div>
                          </form>
                        </b-dropdown-item>
                      </b-dropdown>
                    </div>
                  </div>
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
      </div>

      <!-- Hero content: will be in the middle -->
      <div class="hero-body">
        <div class="container has-text-centered">
          <div class="tile is-ancestor">
            <div class="tile is-vertical is-12">
              <div class="tile">
                <div class="tile is-parent is-vertical">
                  <article class="tile is-child box">
                    <img
                      src="../../public/ibimg.jpg"
                      alt="Bulma: a modern CSS framework based on Flexbox"
                      width="2000"
                      height="3000"
                    />
                  </article>
                </div>
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
                <a>Modifiers</a>
              </li>
              <li>
                <a>Grid</a>
              </li>
              <li>
                <a>Elements</a>
              </li>
              <li>
                <a>Components</a>
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


