<template>
  <v-app style="background-color:#252835;">
    <Navbar />
    <v-main>  
      <Hero /> 
      <Projects /> 
      <About /> 
      <Contact />
    </v-main>
    <Footer />
  </v-app>
</template>

<script>
import Navbar from './components/Navbar';
import Hero from './components/Hero';
import Projects from './components/Projects';
import About from './components/About';
import Contact from './components/Contact';
import Footer from './components/Footer';

export default {
  name: 'App',

  components: {
    Navbar,
    Hero,
    Projects,
    About,
    Contact,
    Footer
  },

  data: () => ({
    //
  }),
};
</script>


<style>

</style>