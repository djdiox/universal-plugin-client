<template>
  <header class="main-header">
    <v-app-bar elevation="8" outlined prominent rounded>
      <v-toolbar-title>Universal Plugin Manager</v-toolbar-title>
      <nuxt-link to="/" exact>
        <v-btn value="recent">
          <span>Home</span>
          <v-icon>mdi-home</v-icon>
        </v-btn>
      </nuxt-link>
      <nuxt-link to="/app-overview" exact>
        <v-btn value="recent">
          <span>Apps</span>
          <v-icon>mdi-apps</v-icon>
        </v-btn>
      </nuxt-link>
    </v-app-bar>
    <!-- <nav>
      <div>
        <nuxt-link to="/" exact> System info </nuxt-link>
      </div>
      <div>
        <nuxt-link to="/apps" exact> Apps </nuxt-link>
      </div>
    </nav> -->
  </header>
</template>

<script>
export default {
  name: 'HeaderComponent'
}
</script>

<style scoped>
.main-header {
  height: 50px;
  display: flex;
  background-color: #364758;
}

nav {
  width: 100%;
  display: flex;
  justify-content: center;
}

nav div {
  height: 100%;
  margin: 0 20px;
  display: flex;
  align-items: center;
}

a {
  font-family: Helvetica, sans-serif;
  color: white;
  font-size: 1rem;
  font-weight: 100;
  text-decoration: underline;
  text-transform: uppercase;
}

a:hover {
  opacity: 0.9;
}
</style>
