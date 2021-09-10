<template>
  <v-container id="about">
    <div class="header">
      <div class="projects-background"></div>
      <div>
        <h1
          class="projects-section drawings d-flex justify-center mt-15 text-center"
          style="text-shadow: 2px 2px 4px #000000;"
        >
          About Me
        </h1>
      </div>
    </div>

    <v-container>
      <v-row class="d-flex justify-center">
        <div class="col-lg-10 col-md-10 col-sm-12 col-xs-12 mt-7">
          <p
            class="skills-title d-flex justify-center"
            style="text-shadow: 2px 2px 4px #000000;"
          >
            Technical Skills
          </p>

          <p class="skills-items">
            <span class="tech-skills-title">Languages:</span> JavaScript[ES6+],
            HTML, CSS, Sass, TypeScript
          </p>
          <p class="skills-items">
            <span class="tech-skills-title">Frameworks & Libraries:</span>
            Vue.js, Vuex, Bootstrap, Tailwind CSS, Vuetify, Vue-Router, Axios,
            Jest
          </p>
          <p class="skills-items">
            <span class="tech-skills-title">Web Technologies:</span>
            Git, Fetch API, NPM, GitHub, ESLint, Babel
          </p>
          <p class="skills-items">
            <span class="tech-skills-title">Tools:</span>
            VScode, Heroku, Figma, Netlify, Chrome DevTools, Vue.js devtools,
            Postman
          </p>
          <p class="skills-items">
            <span class="tech-skills-title">Skills:</span> Responsive Web
            Design, PSD to HTML, Agile, Object Oriented Development, SEO, Web
            Optimization
          </p>
        </div>
      </v-row>
    </v-container>
  </v-container>
</template>

<script>
export default {};
</script>

<style>
.tech-skill-logo {
  max-width: 90px;
}
.skills-title {
  font-family: 'Alegreya Sans', sans-serif;
  font-size: 40px;
  font-weight: 700;
  color: #ffff;
}
.skills-items {
  font-size: 20px;
  color: #ffff;
  font-family: 'Tienne', serif;
  font-weight: 400;
}
.tech-skills-title {
  font-size: 20px;
  color: #e877a6;
  font-family: 'Tienne', serif;
  font-weight: 900;
}
.about-text {
  font-size: 20px;
  color: #ffff;
  font-family: 'Tienne', serif;
  font-weight: 400;
}

@media (max-width: 479px) {
  .skills-items {
    font-size: 17px;
  }
  .about-text {
    font-size: 17px;
  }
}
</style>
