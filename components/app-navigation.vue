<template>
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
            <nuxt-link class="navbar-link" to="/presentation">
              <span class="icon">
                <i class="fas fa-eye" />
              </span>
              <span>Présentation</span>
            </nuxt-link>

            <div class="navbar-dropdown">
              <nuxt-link class="navbar-item" to="/presentation/qui-sommes-nous">
                Qui sommes nous
              </nuxt-link>
              <nuxt-link class="navbar-item" to="/presentation/organisation-du-groupe">
                Organisation du groupe
              </nuxt-link>
              <nuxt-link class="navbar-item" to="/presentation/responsables">
                L'équipe de responsables
              </nuxt-link>
              <hr class="navbar-divider">
              <nuxt-link class="navbar-item" to="/presentation/le-scoutisme">
                Le scoutisme
              </nuxt-link>
              <nuxt-link class="navbar-item" to="/presentation/buts-du-scoutisme">
                But du scoutisme
              </nuxt-link>
            </div>
          </div>

          <!-- ACTIVITES -->
          <div class="navbar-item has-dropdown is-hoverable">
            <nuxt-link class="navbar-link" to="/activites">
              <span class="icon">
                <i class="fas fa-compass" />
              </span>
              <span>Activités</span>
            </nuxt-link>

            <div class="navbar-dropdown">
              <nuxt-link class="navbar-item" to="/activites/prochain-semestre">
                Prochain semestre
              </nuxt-link>
              <hr class="navbar-divider">
              <nuxt-link class="navbar-item" to="/activites/louveteaux">
                Louveteaux (7-11ans)
              </nuxt-link>
              <nuxt-link class="navbar-item" to="/activites/eclaireurs">
                Eclaireurs (12-16ans)
              </nuxt-link>
              <hr class="navbar-divider">
              <nuxt-link class="navbar-item" to="/activites/week-ends">
                Week-ends
              </nuxt-link>
              <nuxt-link class="navbar-item" to="/activites/camps">
                Camps
              </nuxt-link>
              <nuxt-link class="navbar-item" to="/activites/calendrier">
                Calendrier complet
              </nuxt-link>
              <nuxt-link class="navbar-item" to="/activites/lieux-et-horaires">
                Lieux et horaires classique
              </nuxt-link>
              <hr class="navbar-divider">
              <nuxt-link class="navbar-item" to="/activites/infos">
                Infos utiles
              </nuxt-link>
            </div>
          </div>

          <!-- DOCUMENTS -->
          <div class="navbar-item has-dropdown is-hoverable">
            <nuxt-link class="navbar-link" to="/documents">
              <span class="icon">
                <i class="fas fa-file-alt" />
              </span>
              <span>Documents</span>
            </nuxt-link>

            <div class="navbar-dropdown">
              <nuxt-link class="navbar-item" to="/documents/photos">
                Photos
              </nuxt-link>
              <nuxt-link class="navbar-item" to="/documents/nous-rejoindre">
                Nous rejoindre
              </nuxt-link>
              <nuxt-link class="navbar-item" to="/documents/pv">
                PV assemblées générales
              </nuxt-link>
              <hr class="navbar-divider">
              <nuxt-link class="navbar-item" to="/documents/liens-externes">
                Liens externes
              </nuxt-link>
            </div>
          </div>
        </div>

        <div class="navbar-end">
          <!-- Contact -->
          <div class="navbar-item has-dropdown is-hoverable">
            <nuxt-link class="navbar-link" to="/contact/notre-local">
              <span class="icon">
                <i class="fas fa-map-marker-alt" />
              </span>
              <span>Ou / Contact</span>
            </nuxt-link>

            <div class="navbar-dropdown is-right">
              <nuxt-link class="navbar-item" to="/contact/notre-local">
                Notre Local
              </nuxt-link>
              <nuxt-link class="navbar-item" to="/contact/rdv-seances">
                Rendez-vous des séances
              </nuxt-link>
              <hr class="navbar-divider">
              <nuxt-link class="navbar-item" to="/contact">
                Contact
              </nuxt-link>
            </div>
          </div>
          <!-- Search-->
          <search-field />
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
</template>
