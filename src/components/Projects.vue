<template>
  <div id="projects">
    <v-container>
      <v-flex>
      <div class="header">
        <div class="projects-background"></div>
        <div><h1 style="text-shadow: 2px 2px 4px #000000;" class="projects-section d-flex justify-center mt-15 text-center">Featured Projects</h1></div>
      </div>
      <v-item-group>
      <v-container>
        <v-row>
      <div class="col-lg-4 col-md-6 col-sm-6 col-xs-12">
        <v-card
          class="mx-auto"
          max-width="300"
          dark>
          <v-img
          height="200px"
          src="@/assets/open-tabs-landing-page.png"
          >
          </v-img>

            <v-card-subtitle class="pb-0 white--text text-center">
              <p class="project-title">Open Tabs landing Page</p>
            </v-card-subtitle>

          <v-card-text class="white--text" style="overflow-y: auto; height:319px">
            <div class="project-description text-center">I built the landing page from scratch to show the company's missions such as (Saving Rainforests, Preventing Malaria, and Providing Microloans) and to show how to download our browser extension that is the main source of the company's donations. 
            </div>
            <div class="project-description pt-5 text-center" style="font-weight:700;">
            Technologies Used
            </div>   
          <v-list-item>
            <v-list-item-content  class="pb-0 text-center">
              <v-list-item-title class="project-description">HTML/CSS</v-list-item-title>
              <v-list-item-title class="project-description">JavaScript</v-list-item-title>
              <v-list-item-title class="project-description">BoorStrap4</v-list-item-title>
              <v-list-item-title class="project-description">SASS</v-list-item-title>
            </v-list-item-content>
          </v-list-item>

          </v-card-text>

          <v-card-actions class="d-flex justify-center">
            <v-tooltip top close-delay="300" color="secondary">
              <template v-slot:activator="{ on, attrs }">
                <div class="text-center mr-5">
                 <a href="https://relaxant-forearms.000webhostapp.com/" target="_blank"><v-btn style="background-color: #252835;" fab small depressed="true"  dark v-bind="attrs"
                  v-on="on">
                  <v-icon small=""> fas fa-desktop</v-icon>
                  </v-btn></a>
                </div>
              </template>
              <span>View Demo</span>
            </v-tooltip>

     

         <v-tooltip top close-delay="300"  color="secondary">
         <template v-slot:activator="{ on, attrs }">
          <div class="text-center ml-5">
            <a href="https://github.com/lukastars/OpenTabs" target="_blank" class="link-btn">  <v-btn style="background-color: #252835;" fab small depressed="true" dark v-bind="attrs"
                v-on="on">
                <v-icon >fab fa-github</v-icon>
              </v-btn> </a>
            </div>
            </template>
            <span>View Code</span>
          </v-tooltip>



            
          </v-card-actions>
        </v-card>
      </div>
      <div class="col-lg-4 col-md-6 col-sm-6 col-xs-12">
        <v-card
          class="mx-auto"
          max-width="300"
          dark>
          <v-img
          height="200px"
          src="@/assets/open-tabs-blog.png"
          >
          </v-img>

            <v-card-subtitle class="pb-0 white--text text-center">
              <p class="project-title">Open Tabs Blog</p>
            </v-card-subtitle>

          <v-card-text class="white--text" style="overflow-y: auto; height:319px">
            <div class="project-description text-center">I made a blog for OpenTabs to share its latest updates and news with the world in a simple and elegant style.
            </div>
            <div class="project-description pt-5 text-center" style="font-weight:700;">
            Technologies Used
            </div>   
          <v-list-item>
            <v-list-item-content  class="pb-0 text-center">
              <v-list-item-title class="project-description">HTML/CSS</v-list-item-title>
              <v-list-item-title class="project-description">JavaScript</v-list-item-title>
              <v-list-item-title class="project-description">BoorStrap4</v-list-item-title>
              <v-list-item-title class="project-description">SASS</v-list-item-title>
            </v-list-item-content>
          </v-list-item>

          </v-card-text>

          <v-card-actions class="d-flex justify-center">
            <v-tooltip top close-delay="300" color="secondary">
              <template v-slot:activator="{ on, attrs }">
                <div class="text-center mr-5">
                <a href="https://relaxant-forearms.000webhostapp.com/blog/" target="_blank" class="link-btn">  <v-btn style="background-color: #252835;" fab small depressed="true"  dark v-bind="attrs"
                  v-on="on">
                  <v-icon small=""> fas fa-desktop</v-icon>
                  </v-btn></a>
                </div>
              </template>
              <span>View Demo</span>
            </v-tooltip>

     

         <v-tooltip top close-delay="300"  color="secondary">
         <template v-slot:activator="{ on, attrs }">
          <div class="text-center ml-5">
            <a href="https://github.com/lukastars/OpenTabs" target="_blank" class="link-btn">  <v-btn style="background-color: #252835;" fab small depressed="true" dark v-bind="attrs"
                v-on="on">
                <v-icon >fab fa-github</v-icon>
              </v-btn></a>
            </div>
            </template>
            <span>View Code</span>
          </v-tooltip>



            
          </v-card-actions>
        </v-card>
      </div>
      <div class="col-lg-4 col-md-6 col-sm-6 col-xs-12">
        <v-card
          class="mx-auto"
          max-width="300"
          dark>
          <v-img
          height="200px"
          src="@/assets/apex-tracker-app.png"
          >
          </v-img>

            <v-card-subtitle class="pb-0 white--text text-center">
              <p class="project-title">Apex Legends Tracker App</p>
            </v-card-subtitle>

          <v-card-text class="white--text" style="overflow-y: auto; height:319px">
            <div class="project-description text-center">A Full-Stack web application that tracks Apex Legends players status. I got the API that show players data from tracker.gg, Then I used Postman to test the API by createing HTTP/s requests and reading their responses. Then I built the Fron-End from scratch using Vue.js with Vue-router
            </div>
            <div class="project-description pt-5 text-center" style="font-weight:700;">
            Technologies Used
            </div>   
            <div class="d-flex justify-center">
              <div>
                <div class="project-description pt-3 text-center" style="font-weight:700;">
            Front-End
            </div> 
          <v-list-item>
            <v-list-item-content  class="pb-0 text-center">
              <v-list-item-title class="project-description">Vue.js with Vue-router</v-list-item-title>
              <v-list-item-title class="project-description">HTML/CSS/JavaScript</v-list-item-title>             
              <v-list-item-title class="project-description">Vue Toasted</v-list-item-title>             
            </v-list-item-content>
          </v-list-item>
          </div>
           <v-list-item>
             <div>
               <div class="project-description pt-3 text-center" style="font-weight:700;">
            Back-End
            </div> 
            <v-list-item-content  class="pb-0 text-center">
              <v-list-item-title class="project-description">Node.js</v-list-item-title>
              <v-list-item-title class="project-description">Express.js</v-list-item-title>
              <v-list-item-title class="project-description">Postman, Axios</v-list-item-title>
            </v-list-item-content>
            </div>
          </v-list-item>
          </div>

          </v-card-text>

          <v-card-actions class="d-flex justify-center">
            <v-tooltip top close-delay="300" color="secondary">
              <template v-slot:activator="{ on, attrs }">
                <div class="text-center mr-5">
                <a href="https://hidden-basin-62213.herokuapp.com/" target="_blank" class="link-btn">  <v-btn style="background-color: #252835;" fab small depressed="true"  dark v-bind="attrs"
                  v-on="on">
                  <v-icon small="" color=""> fas fa-desktop</v-icon>
                  </v-btn></a>
                </div>
              </template>
              <span>View Demo</span>
            </v-tooltip>

     

         <v-tooltip top close-delay="300"  color="secondary">
         <template v-slot:activator="{ on, attrs }">
          <div class="text-center ml-5">
            <a href="https://github.com/lukastars/Apex-Legends-Tracker" target="_blank" class="link-btn">  <v-btn style="background-color: #252835;" fab small depressed="true" dark v-bind="attrs"
                v-on="on">
                <v-icon >fab fa-github</v-icon>
              </v-btn></a>
            </div>
            </template>
            <span>View Code</span>
          </v-tooltip>



            
          </v-card-actions>
        </v-card>
      </div>
      <div class="col-lg-4 col-md-6 col-sm-6 col-xs-12">
        <v-card
          class="mx-auto"
          max-width="300"
          dark>
          <v-img
          height="200px"
          src="@/assets/digital-agency.png"
          >
          </v-img>

            <v-card-subtitle class="pb-0 white--text text-center">
              <p class="project-title">Digital Agency Website</p>
            </v-card-subtitle>

          <v-card-text class="white--text" style="overflow-y: auto; height:319px">
            <div class="project-description text-center">A fully responsive modern and elegant website for a Digital Agency selling almost any kind of services.
            </div>
            <div class="project-description pt-5 text-center" style="font-weight:700;">
            Technologies Used
            </div>   
          <v-list-item>
            <v-list-item-content  class="pb-0 text-center">
              <v-list-item-title class="project-description">HTML/CSS</v-list-item-title>
              <v-list-item-title class="project-description">JavaScript</v-list-item-title>
              <v-list-item-title class="project-description">BoorStrap4</v-list-item-title>
              <v-list-item-title class="project-description">SASS</v-list-item-title>
            </v-list-item-content>
          </v-list-item>

          </v-card-text>

          <v-card-actions class="d-flex justify-center">
            <v-tooltip top close-delay="300" color="secondary">
              <template v-slot:activator="{ on, attrs }">
                <div class="text-center mr-5">
                <a href="https://lukastars.github.io/Digital-Agency/" target="_blank" class="link-btn">  <v-btn style="background-color: #252835;" fab small depressed="true"  dark v-bind="attrs"
                  v-on="on">
                  <v-icon small="" color=""> fas fa-desktop</v-icon>
                  </v-btn></a>
                </div>
              </template>
              <span>View Demo</span>
            </v-tooltip>

     

         <v-tooltip top close-delay="300"  color="secondary">
         <template v-slot:activator="{ on, attrs }">
          <div class="text-center ml-5">
            <a href="https://github.com/lukastars/Digital-Agency" target="_blank" class="link-btn">  <v-btn style="background-color: #252835;" fab small depressed="true" dark v-bind="attrs"
                v-on="on">
                <v-icon >fab fa-github</v-icon>
              </v-btn></a>
            </div>
            </template>
            <span>View Code</span>
          </v-tooltip>



            
          </v-card-actions>
        </v-card>
      </div>
      </v-row>
      </v-container>
      </v-item-group>
      </v-flex>
      <div class="d-flex justify-center mt-12">
     <a href="https://github.com/lukastars?tab=repositories" class="link-btn" target="_blank"><v-btn rounded="true" x-large="true">
          <span class="projects-btn">More Projects</span>
        </v-btn></a>
      </div> 
    </v-container>
 </div>  
</template>

<script>
export default {

}
</script>

<style>
.projects-section {
  font-size: 130px;
  color: #ffff;
  font-family: 'Alegreya Sans', sans-serif;
  font-weight: 900;
  position: relative;
  z-index: 1;
}
.header {
  position: relative;
}

.project-title {
  font-size: 20px;
  font-family: 'Alegreya Sans', sans-serif;
  font-weight: 700;
}
.projects-background {
  background-image: url("../assets/drawings.svg");
  background-position: 0% 0%;
  background-size: 61%;
  background-repeat: no-repeat;
  position: absolute;
  height: 100%;
  width: 100%;
  z-index: 0;
  animation: float 7s ease-in-out infinite;
}

.project-description {
  font-size: 16px !important;
  font-family:'Alegreya Sans', sans-serif;
  font-weight: 400;
}

@media (max-width: 1265px) {
  .projects-section {
  font-size: 100px;
  }
}
@media (max-width: 479px) {
  .projects-section {
  font-size: 78px;
  }
  .projects-background {
    background-size: 100%;
  }
}

</style>