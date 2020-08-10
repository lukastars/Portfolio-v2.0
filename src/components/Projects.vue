<template>
  <div id="projects">
    <v-container>
      <v-flex>
      <div class="header">
        <div class="projects-background"></div>
        <div><h1 style="text-shadow: 2px 2px 4px #000000;" class="projects-section d-flex justify-center mt-15 text-center">Featured Projects</h1></div>
      </div>
      <v-container>
        <v-row>
      <div class="col-lg-4 col-md-6 col-sm-6 col-xs-12">
        <v-card
          class="mx-auto"
          max-width="300"
          dark>
          <v-img
          height="200px"
          src="https://cdn.vuetifyjs.com/images/cards/docks.jpg"
          >
          </v-img>

            <v-card-subtitle class="pb-0 white--text text-center">
              <p class="project-title">Digital Agency Website</p>
            </v-card-subtitle>

          <v-card-text class="white--text">
            <div class="project-description text-center">This is a fully responsive & modern website for digital agencies
            </div>
            <div class="project-description pt-5 text-center" style="font-weight:700;">
            Technologies Used
            </div>   
          <v-list-item>
            <v-list-item-content  class="pb-0 text-center">
              <v-list-item-title class="project-description">HTML/CSS</v-list-item-title>
              <v-list-item-title class="project-description">BoorStrap4</v-list-item-title>
              <v-list-item-title class="project-description">JavaScript</v-list-item-title>
            </v-list-item-content>
          </v-list-item>

          </v-card-text>

          <v-card-actions class="d-flex justify-center">
            <v-tooltip top close-delay="300" color="secondary">
              <template v-slot:activator="{ on, attrs }">
                <div class="text-center mr-5">
                  <v-btn style="background-color: #252835;" fab small depressed="true"  dark v-bind="attrs"
                  v-on="on">
                  <v-icon small=""> fas fa-desktop</v-icon>
                  </v-btn>
                </div>
              </template>
              <span>View Demo</span>
            </v-tooltip>

     

         <v-tooltip top close-delay="300"  color="secondary">
         <template v-slot:activator="{ on, attrs }">
          <div class="text-center ml-5">
              <v-btn style="background-color: #252835;" fab small depressed="true" dark v-bind="attrs"
                v-on="on">
                <v-icon >fab fa-github</v-icon>
              </v-btn>
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
          src="https://cdn.vuetifyjs.com/images/cards/docks.jpg"
          >
          </v-img>

            <v-card-subtitle class="pb-0 white--text text-center">
              <p class="project-title">Digital Agency Website</p>
            </v-card-subtitle>

          <v-card-text class="white--text">
            <div class="project-description text-center">This is a fully responsive & modern website for digital agencies
            </div>
            <div class="project-description pt-5 text-center" style="font-weight:700;">
            Technologies Used
            </div>   
          <v-list-item>
            <v-list-item-content  class="pb-0 text-center">
              <v-list-item-title class="project-description">HTML/CSS</v-list-item-title>
              <v-list-item-title class="project-description">BoorStrap4</v-list-item-title>
              <v-list-item-title class="project-description">JavaScript</v-list-item-title>
            </v-list-item-content>
          </v-list-item>

          </v-card-text>

          <v-card-actions class="d-flex justify-center">
            <v-tooltip top close-delay="300" color="secondary">
              <template v-slot:activator="{ on, attrs }">
                <div class="text-center mr-5">
                  <v-btn style="background-color: #252835;" fab small depressed="true"  dark v-bind="attrs"
                  v-on="on">
                  <v-icon small=""> fas fa-desktop</v-icon>
                  </v-btn>
                </div>
              </template>
              <span>View Demo</span>
            </v-tooltip>

     

         <v-tooltip top close-delay="300"  color="secondary">
         <template v-slot:activator="{ on, attrs }">
          <div class="text-center ml-5">
              <v-btn style="background-color: #252835;" fab small depressed="true" dark v-bind="attrs"
                v-on="on">
                <v-icon >fab fa-github</v-icon>
              </v-btn>
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
          src="https://cdn.vuetifyjs.com/images/cards/docks.jpg"
          >
          </v-img>

            <v-card-subtitle class="pb-0 white--text text-center">
              <p class="project-title">Digital Agency Website</p>
            </v-card-subtitle>

          <v-card-text class="white--text">
            <div class="project-description text-center">This is a fully responsive & modern website for digital agencies
            </div>
            <div class="project-description pt-5 text-center" style="font-weight:700;">
            Technologies Used
            </div>   
          <v-list-item>
            <v-list-item-content  class="pb-0 text-center">
              <v-list-item-title class="project-description">HTML/CSS</v-list-item-title>
              <v-list-item-title class="project-description">BoorStrap4</v-list-item-title>
              <v-list-item-title class="project-description">JavaScript</v-list-item-title>
            </v-list-item-content>
          </v-list-item>

          </v-card-text>

          <v-card-actions class="d-flex justify-center">
            <v-tooltip top close-delay="300" color="secondary">
              <template v-slot:activator="{ on, attrs }">
                <div class="text-center mr-5">
                  <v-btn style="background-color: #252835;" fab small depressed="true"  dark v-bind="attrs"
                  v-on="on">
                  <v-icon small="" color=""> fas fa-desktop</v-icon>
                  </v-btn>
                </div>
              </template>
              <span>View Demo</span>
            </v-tooltip>

     

         <v-tooltip top close-delay="300"  color="secondary">
         <template v-slot:activator="{ on, attrs }">
          <div class="text-center ml-5">
              <v-btn style="background-color: #252835;" fab small depressed="true" dark v-bind="attrs"
                v-on="on">
                <v-icon >fab fa-github</v-icon>
              </v-btn>
            </div>
            </template>
            <span>View Code</span>
          </v-tooltip>



            
          </v-card-actions>
        </v-card>
      </div>
      </v-row>
      </v-container>
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