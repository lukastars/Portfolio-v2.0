<template>
  <v-container id="about">
    <div class="header">
        <div class="projects-background"></div>
        <div><h1 class="projects-section drawings d-flex justify-center mt-15 text-center" style="text-shadow: 2px 2px 4px #000000;">About Me</h1></div>
      </div>
     
    <v-container>
      <v-row class="d-flex justify-center">
        <div class="col-lg-6 col-md-10 col-sm-12 col-xs-12 d-flex align-center">
          <p class="about-text text-center ">I've studied Business Information Systems in University but I found more passion and enjoyment in Web Development compared to BIS jobs, I am working on getting more into the Industry because it makes excellent use of my critical thinking, problem-solving, creativity skills and my fast learning capability makes me easily learn, adapt and stay up to date with the latest technologies.  </p>

        </div>
        <div class="col-lg-6 col-md-10 col-sm-12 col-xs-12 ">
          <p class="about-text text-center" >Some Technologies I've Worked With</p>
          <div >
            <img src="@/assets/vue.png" alt="" class="tech-skill-logo col-lg-2" >
            <img src="@/assets/javascript.png" alt="" class="tech-skill-logo   col-lg-2 col-md-2 col-sm-3">
            <img src="@/assets/html5.png" alt="" class="tech-skill-logo col-lg-2 col-md-2 col-sm-3">
            <img src="@/assets/css3.png" alt="" class="tech-skill-logo col-lg-2 col-md-2 col-sm-3">
            <img src="@/assets/bootstrap.png" alt="" class="tech-skill-logo col-lg-2 col-md-2 col-sm-3">
             <img src="@/assets/sass.png" alt="" class="tech-skill-logo col-lg-2 col-md-2 col-sm-3">
             <img src="@/assets/typescript.png" alt="" class="tech-skill-logo col-lg-2 col-md-2 col-sm-3">
             <img src="@/assets/node-js.png" alt="" class="tech-skill-logo col-lg-2 col-md-2 col-sm-3">
             <img src="@/assets/heroku.png" alt="" class="tech-skill-logo col-lg-2 col-md-2 col-sm-3">
             <img src="@/assets/jquery.png" alt="" class="tech-skill-logo col-lg-2 col-md-2 col-sm-3">
             <img src="@/assets/github.png" alt="" class="tech-skill-logo col-lg-2 col-md-2 col-sm-3">
             <img src="@/assets/visualstudio.png" alt="" class="tech-skill-logo col-lg-2 col-md-2 col-sm-3">
          </div>
        </div>
        <div class="col-lg-10 col-md-10 col-sm-12 col-xs-12 mt-7">
          
          <p class="skills-title d-flex justify-center" style="text-shadow: 2px 2px 4px #000000;">Technical Skills</p>

          <p class="skills-items"><span class="tech-skills-title">Languages:</span> JavaScript[ES6+], HTML, CSS, Sass, TypeScript ,Node.js</p>
          <p class="skills-items"><span class="tech-skills-title">Frameworks & Libraries:</span> Vue.js, JQuery, Bootstrap, Express.js</p>
          <p class="skills-items"><span class="tech-skills-title">Skills:</span> Responsive Web Design, PSD to HTML, Agile, Accessibility, Web Optimization</p>
          <p class="skills-items"><span class="tech-skills-title">Web Technologies:</span> REST API, GraphQL, Express</p>
          <p class="skills-items"><span class="tech-skills-title">Tools:</span> Git, VScode, ESLint, Babel, Balsamiq, Heroku, Netlify, GitHub, Chrome DevTools</p>

        </div>
      </v-row>
    </v-container> 
  </v-container>
</template>

<script>
export default {

}
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
  font-family:'Tienne', serif;
  font-weight: 400;
}
.tech-skills-title {
  font-size: 20px;
  color: #e877a6;
  font-family:'Tienne', serif;
  font-weight: 900;
}
.about-text {
  font-size: 20px;
  color: #ffff;
  font-family:'Tienne', serif;
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