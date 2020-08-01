<template>
  <div>
    <nav class="navbar is-spaced has-shadow" role="navigation" aria-label="main navigation">
      <div class="container">
        <div class="navbar-brand">
          <nuxt-link class="navbar-item" to="/">
            <img src="~/assets/logo.svg" width="112" height="40">
          </nuxt-link>

          <a
            role="button"
            class="navbar-burger burger"
            aria-label="menu"
            aria-expanded="false"
            data-target="navbarBasicExample"
          >
            <span aria-hidden="true" />
            <span aria-hidden="true" />
            <span aria-hidden="true" />
          </a>
        </div>

        <div id="navbarBasicExample" class="navbar-menu">
          <div class="navbar-start">
            <!-- PRESENTATION -->
            <div class="navbar-item has-dropdown is-hoverable">
              <a class="navbar-link">
                <span class="icon">
                  <i class="fas fa-eye" />
                </span>
                <span>Présentation</span>
              </a>

              <div class="navbar-dropdown">
                <a class="navbar-item">Photos</a>
                <a class="navbar-item">Nous rejoindre</a>
                <a class="navbar-item">PV assemblées générales</a>
                <hr class="navbar-divider">
                <a class="navbar-item">Liens externes</a>
              </div>
            </div>

            <!-- ACTIVITES -->
            <div class="navbar-item has-dropdown is-hoverable">
              <a class="navbar-link">
                <span class="icon">
                  <i class="fas fa-compass" />
                </span>
                <span>Activités</span>
              </a>

              <div class="navbar-dropdown">
                <a class="navbar-item">Photos</a>
                <a class="navbar-item">Nous rejoindre</a>
                <a class="navbar-item">PV assemblées générales</a>
                <hr class="navbar-divider">
                <a class="navbar-item">Liens externes</a>
              </div>
            </div>

            <!-- DOCUMENTS -->
            <div class="navbar-item has-dropdown is-hoverable">
              <a class="navbar-link">
                <span class="icon">
                  <i class="fas fa-file-alt" />
                </span>
                <span>Documents</span>
              </a>

              <div class="navbar-dropdown">
                <a class="navbar-item">Photos</a>
                <a class="navbar-item">Nous rejoindre</a>
                <a class="navbar-item">PV assemblées générales</a>
                <hr class="navbar-divider">
                <a class="navbar-item">Liens externes</a>
              </div>
            </div>
          </div>

          <div class="navbar-end">
            <a class="navbar-item">
              <span class="icon">
                <i class="fas fa-map-marker-alt" />
              </span>
              <span>Contact / Ou</span>
            </a>
            <div class="navbar-item">
              <div class="buttons">
                <a class="button is-light">
                  <span class="icon">
                    <i class="fas fa-user" />
                  </span>
                </a>
              </div>
            </div>
          </div>
        </div>
      </div>
    </nav>
    <div class="bd-main">
      <div class="aside-background" />
      <Nuxt />
    </div>
    <footer class="footer">
      <div class="container">
        <h1 class="title">
          Hello les amis
        </h1>
      </div>
    </footer>
  </div>
</template>
