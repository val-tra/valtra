<template>
  <div class="container">
    <div class="bd-duo">
      <aside aside class="menu bd-aside">
        <p class="menu-label">
          Résumé
        </p>
        <ul class="menu-list">
          <li>
            <nuxt-link to="/activites">
              Nos activités
            </nuxt-link>
          </li>
          <li>
            <nuxt-link to="/activites/prochain-semestre">
              Prochain semestre
            </nuxt-link>
          </li>
        </ul>
        <p class="menu-label">
          Branches
        </p>
        <ul class="menu-list">
          <li>
            <nuxt-link to="/activites/louveteaux">
              Louveteaux (7-11 ans)
            </nuxt-link>
          </li>
          <li>
            <nuxt-link to="/activites/eclaireurs">
              Eclaireurs (12-16 ans)
            </nuxt-link>
          </li>
        </ul>
        <p class="menu-label">
          Toutes les activités
        </p>
        <ul class="menu-list">
          <li>
            <nuxt-link to="/activites/week-ends">
              Week-ends
            </nuxt-link>
          </li>
          <li>
            <nuxt-link to="/activites/camps">
              Camps
            </nuxt-link>
          </li>
          <li>
            <nuxt-link to="/activites/calendrier">
              Calendrier complet
            </nuxt-link>
          </li>
          <li>
            <nuxt-link to="/activites/lieux-et-horaires">
              Lieux et horaires classique
            </nuxt-link>
          </li>
        </ul>
        <p class="menu-label">
          Infos utiles
        </p>
        <ul class="menu-list">
          <li>
            <nuxt-link to="/activites/infos">
              Infos utiles
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
