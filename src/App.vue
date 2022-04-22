<template>
  <div id="app">
    <Home />
    <div class="second">
      <About />
      <Skills />
      <Portfolio />
      <Contact />
      <Footer />
      </div>
  </div>
</template>

<script>
import Home from "./views/HomeView.vue";
import About from "./views/AboutView.vue";
import Skills from "./views/SkillsView.vue";
import Portfolio from "./views/PortfolioView.vue";
import Contact from "./views/ContactView.vue";
import Footer from "./views/FooterView.vue";

export default {
  name: "App",
  components: {
    Home,
    About,
    Skills,
    Portfolio,
    Contact,
    Footer,
  },
};
</script>

<style lang="scss">


$headings-color: #E3A905;
$white-color: #ffffff;
$black-color: #000000;
$gray-color: #707070;


  .second{
    background-image: linear-gradient( #4e4e4eda, #000000d5);
  }



  #about, #skills, #portfolio, #contact{
    height: 100vh;
    width: auto;
    min-height: 100vh;
}

.about h1, .skills h1, .portfolio h1, .contact h1{
    font-weight: bold;
    text-transform: uppercase;
    font-size: 1.9rem;
    color: $headings-color;
}

.section-header {
    padding-bottom: 2rem;
}

article .container-fluid .flex-col {
    padding: 2rem;
}

article {
    min-height: 100%;
    width: 100%;
    background-size: cover;
    text-align: center;
    position: relative;
    padding: 1rem;
}
  
article .container-fluid {
    padding: 1rem;
    margin: 4rem auto;
}
  
article .container-fluid .flex-col {
    padding: 2rem;
}
  
article .list-group-item {
    background-color: inherit;
}

</style>
