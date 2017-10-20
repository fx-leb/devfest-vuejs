<template>
  <div class="navbar navbar-inverse">
    <div class="container-fluid">
      <div class="navbar-header">
        <a class="navbar-brand">
          <!-- Lien vers la page "liste des séries" -->
          <router-link to="/">Home</router-link>
        </a>
      </div>
      <ul class="nav navbar-nav navbar-right">
        <li>
          <!-- Lien vers la page "liste des séries" -->
          <router-link to="/">Liste des séries</router-link>
        </li>
        <li>
          <!-- Lien vers la page "favoris" -->
          <router-link to="/favorites">Favoris</router-link>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
}
</script>

<style>
</style>