<template>
  <div>
    <Navbar />
    <Home />
    <About />
    <Resume />
    <Projects />
    <ProjectDetails />
    <Testimonials />
    <Contact />
    <Footer />
  </div>
</template>

<script>
import Navbar from "./components/Navbar.vue";
import Home from "./components/Home.vue";
import About from "./components/About.vue";
import Resume from "./components/Resume.vue";
import Projects from "./components/Projects.vue";
import Testimonials from "./components/Testimonials.vue";
import Contact from "./components/Contact.vue";
import Footer from "./components/Footer.vue";

export default {
  name: "App",

  components: {
    Navbar,
    Home,
    About,
    Resume,
    Projects,
    Testimonials,
    Contact,
    Footer
  },
};
</script>

<style scoped>


body {
  background: #f2f2f2;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  max-width: 600px;
  margin: auto;
  color: #555;
  padding: 158px;
}


div {
  text-align: center;
}

@media screen and (min-width:346px){
  .name{
    display: none;
  }
}
</style>
