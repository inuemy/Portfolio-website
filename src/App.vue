<template>
  <v-app>
    <Header/>
    <v-main>
      <TopPage/>
      <Profile/>
      <Portfolio/>
      <Contact/>
    </v-main>
    <Footer/>
  </v-app>
</template>

<script>
import Header from './components/Header.vue'
import TopPage from './components/TopPage.vue'
import Profile from './components/Profile.vue'
import Portfolio from './components/Portfolio.vue'
import Contact from './components/Contact.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Header,
    TopPage,
    Profile,
    Portfolio,
    Contact,
    Footer
  },

  data: () => ({
    //
  }),
}
</script>
