<script>
import TopPage from './components/TopPage.vue'
import Profile from './components/Profile.vue'
import Portfolio from './components/Portfolio.vue'
import Contact from './components/Contact.vue'

export default {
  name: 'App',
  components: {
    TopPage,
    Profile,
    Portfolio,
    Contact
  },

  data: () => ({
    //
  }),
}
</script>

<template>
  <v-app>
    <v-app-bar>
      <v-toolber-title>
        <p class="title">Mayu's Room</p>
      </v-toolber-title>
      <v-spacer></v-spacer>
      <v-toolbar-items class="toolbar-items">
        <v-btn text href="#profile-section">Profile</v-btn>
        <v-btn text href="#portfolio-section">Portfolio</v-btn>
        <v-btn text href="#contact-section">Contact</v-btn>
      </v-toolbar-items>
    </v-app-bar>
    <v-main>
      <TopPage/>
      <Profile/>
      <Portfolio/>
      <Contact/>
    </v-main>
    <v-footer color="grey">
        Mayu's Room
    </v-footer>
  </v-app>
</template>

<style>
.title {
  margin: 10px 0px 10px 30px;
  font-size: 25px;;
}
.toolbar-items {
  margin: 0px 30px 0px 0px;
}
.v-main {
  margin: 20px;
}
</style>