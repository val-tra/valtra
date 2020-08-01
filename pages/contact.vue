<template>
  <div class="container">
    <div class="bd-duo">
      <aside aside class="menu bd-aside">
        <ul class="menu-list">
          <li>
            <nuxt-link to="/contact/notre-local">
              Notre local
            </nuxt-link>
          </li>
          <li>
            <nuxt-link to="/contact/rdv-seances">
              Rendez-vous des séances
            </nuxt-link>
          </li>
          <li>
            <nuxt-link to="/contact">
              Nous contacter
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
