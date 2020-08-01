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
                <a class="navbar-item">Qui sommes nous</a>
                <a class="navbar-item">Organisation du groupe</a>
                <a class="navbar-item">L'équipe de responsables</a>
                <hr class="navbar-divider">
                <a class="navbar-item">Le scoutisme</a>
                <a class="navbar-item">But du scoutisme</a>
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
                <a class="navbar-item">Prochain semestre</a>
                <hr class="navbar-divider">
                <a class="navbar-item">Louveteaux (7-11ans)</a>
                <a class="navbar-item">Eclaireurs (12-16ans)</a>
                <hr class="navbar-divider">
                <a class="navbar-item">Week-ends</a>
                <a class="navbar-item">Camps</a>
                <a class="navbar-item">Calendrier complet</a>
                <a class="navbar-item">Lieux et horaires classique</a>
                <hr class="navbar-divider">
                <a class="navbar-item">Infos utiles</a>
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
            <!-- Contact -->
            <div class="navbar-item has-dropdown is-hoverable">
              <a class="navbar-link">
                <span class="icon">
                  <i class="fas fa-map-marker-alt" />
                </span>
                <span>Contact / Ou</span>
              </a>

              <div class="navbar-dropdown is-right">
                <a class="navbar-item">Notre Local</a>
                <a class="navbar-item">Rendez-vous des séances</a>
                <hr class="navbar-divider">
                <a class="navbar-item">Contact</a>
              </div>
            </div>
            <!-- LOG IN -->
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
