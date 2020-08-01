<template>
  <div class="container">
    <div class="bd-duo">
      <aside aside class="menu bd-aside">
        <ul class="menu-list">
          <li>
            <nuxt-link to="/documents">
              Documents divers
            </nuxt-link>
          </li>
          <li>
            <nuxt-link to="/documents/photos">
              Photos
            </nuxt-link>
          </li>
          <li>
            <nuxt-link to="/documents/nous-rejoindre">
              Nous rejoindre
            </nuxt-link>
          </li>
          <li>
            <nuxt-link to="/documents/pv">
              PV's assemblées générales
            </nuxt-link>
          </li>
          <li>
            <nuxt-link to="/documents/liens-externes">
              Liens externes
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
