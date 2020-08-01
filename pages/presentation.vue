<template>
  <div class="container">
    <div class="bd-duo">
      <aside aside class="menu bd-aside">
        <p class="menu-label">
          Le groupe
        </p>
        <ul class="menu-list">
          <li>
            <nuxt-link to="/presentation">
              Présentation
            </nuxt-link>
          </li>
          <li>
            <nuxt-link to="/presentation/qui-sommes-nous">
              Qui sommes nous
            </nuxt-link>
          </li>
          <li>
            <nuxt-link to="/presentation/organisation-du-groupe">
              Organisation du groupe
            </nuxt-link>
          </li>
          <li>
            <nuxt-link to="/presentation/responsables">
              L'équipe de responsables
            </nuxt-link>
          </li>
        </ul>
        <p class="menu-label">
          Le scoutisme
        </p>
        <ul class="menu-list">
          <li>
            <nuxt-link to="/presentation/le-scoutisme">
              Le scoutisme
            </nuxt-link>
          </li>
          <li>
            <nuxt-link to="/presentation/buts-du-scoutisme">
              But du scoutisme
            </nuxt-link>
          </li>
        </ul>
      </aside>
      <div class="bd-lead">
        <nuxt-child />
      </div>
    </div>
  </div>
</template>
