<template>
  <v-container class="d-flex justify-center">
        <nav>
          <v-app-bar  app fixed flat style="background-color:transparent;" class="pt-5">
      <v-toolbar flat fixed    class="rounded" style="background-color:#e877a6;">
        <v-toolbar-logo>
          <div class="d-flex  align-center">
           <span class="logo-text text-color">Ali.</span>
                  <div class="hidden-sm-and-down ml-3">
                     <a href="https://www.linkedin.com/in/ali-a-81ab8112a" target="_blank" class="link-btn"> <v-btn x-small style="background-color: #252835;" fab  depressed="true" dark v-bind="attrs"
                        v-on="on" class="mr-2">
                        <v-icon  color="error">fab fa-linkedin</v-icon>
                    </v-btn></a>
                     <a href="https://github.com/lukastars" target="_blank" class="link-btn"> <v-btn x-small style="background-color: #252835;" fab  depressed="true" dark v-bind="attrs"
                        v-on="on" class="mr-2">
                        <v-icon  color="error">fab fa-github</v-icon>
                      </v-btn></a>
                       <a href="mailto:bonger2014@gmail.com" target="_blank" class="link-btn"> <v-btn x-small style="background-color: #252835;" fab  depressed="true" dark v-bind="attrs"
                        v-on="on">
                        <v-icon  color="error">far fa-envelope</v-icon>
                      </v-btn></a>
              </div>
            </div>
        </v-toolbar-logo>
        <v-spacer></v-spacer>
        <div class="hidden-md-and-up">
          <v-menu bottom left>
            <template v-slot:activator="{ on, attrs }">
              <v-btn
                dark
                icon
                v-bind="attrs"
                v-on="on"
              >
                <v-icon color="secondary">fas fa-bars</v-icon>
              </v-btn>
            </template>

            <v-list color="accent">
                  <v-list-item>
                    <v-btn text="true" @click="$vuetify.goTo(target[0], options)">
                <span class="text-color">Projects</span>
              </v-btn>
                  </v-list-item>
                  <v-list-item>
              <v-btn text="true" @click="$vuetify.goTo(target[1], options)">
                <span class="text-color">About</span>
              </v-btn>
              </v-list-item>
              <v-list-item>
              <a href="https://drive.google.com/file/d/1D6Le7SFhZlz-GRmyP9rqvxFM735CB5cd/view?usp=sharing" target="_blank" class="link-btn"><v-btn text="true">
                <span class="text-color">Résumé</span>
              </v-btn></a>
                  </v-list-item>
                  <v-list-item>
                   <a href="https://www.linkedin.com/in/ali-a-81ab8112a" target="_blank" class="link-btn"><v-btn x-small style="background-color: #252835;" fab  depressed="true" dark v-bind="attrs"
                    v-on="on" class="mr-2">
                    <v-icon  color="error">fab fa-linkedin</v-icon>
                </v-btn></a>
                <a href="https://github.com/lukastars" target="_blank" class="link-btn"><v-btn x-small style="background-color: #252835;" fab  depressed="true" dark v-bind="attrs"
                    v-on="on" class="mr-2">
                    <v-icon  color="error">fab fa-github</v-icon>
                  </v-btn></a>
                    <a href="mailto:bonger2014@gmail.com" target="_blank" class="link-btn"><v-btn x-small style="background-color: #252835;" fab  depressed="true" dark v-bind="attrs"
                v-on="on">
                <v-icon  color="error">far fa-envelope</v-icon>
              </v-btn></a>
              </v-list-item>
            </v-list>
          </v-menu>
          </div>
          <div class="hidden-sm-and-down">
          
            <v-btn text="true" right class="mr-2" @click="$vuetify.goTo(target[0], options)">
              <span class="text-color">Projects</span>
            </v-btn>
            <v-btn text="true" right class="mr-2" @click="$vuetify.goTo(target[1], options)">
              <span class="text-color">About</span>
            </v-btn>
            <a href="https://drive.google.com/file/d/1D6Le7SFhZlz-GRmyP9rqvxFM735CB5cd/view?usp=sharing" target="_blank" class="link-btn"> <v-btn text="true" right>
              <span class="text-color">Résumé</span>
            </v-btn> </a>
          
        </div>
      </v-toolbar>
      </v-app-bar>
      </nav>
  </v-container>
  
</template>

<script>
const easings = {
  linear: '',
  easeInQuad: '',
  easeOutQuad: '',
  easeInOutQuad: '',
  easeInCubic: '',
  easeOutCubic: '',
  easeInOutCubic: '',
  easeInQuart: '',
  easeOutQuart: '',
  easeInOutQuart: '',
  easeInQuint: '',
  easeOutQuint: '',
  easeInOutQuint: ''
}
export default {
  data () {
    return {
      type: 'selector',
      selector: ['#projects', '#about'],
      selected: 'Button',
      duration: 700,
      offset: -45,
      easing: 'easeInOutQuad',
      easings: Object.keys(easings),
    }
  },
  computed: {
    target () {
      const value = this[this.type]
      if (!isNaN(value)) return Number(value)
      else return value
    },
    options () {
      return {
        duration: this.duration,
        offset: this.offset,
        easing: this.easing,
      }
    },
  },
}
</script>

<style>
.link-btn {
  text-decoration: none;
}

nav span {
  font-family: 'Alegreya Sans', sans-serif;
  font-weight: 900;
  text-decoration: none;
  font-size: 16px;
  
}
.logo-text {
  font-size: 50px;
  font-weight: 900;
}
.text-color {
  color: #252835;
}
</style>