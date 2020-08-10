<template>
<div class="wave-section">
  <v-container class="d-flex justify-center">
    <v-flex class="text-center col-lg-7 col-md-9 col-sm-12">
    <h1 class="contact-title mt-15 text-center" style="text-shadow: 2px 2px 4px #000000;">Wanna chat?</h1> 
    <p class="contact-p" style="text-shadow: 2px 2px 4px #000000;">Whether you have an idea for a project or just want to chat, feel free to shoot me an email!</p>
    <div class="pb-15">
    <a href="https://www.linkedin.com/in/ali-a-81ab8112a" target="_blank" class="link-btn">  <v-btn large style="background-color: #252835;" fab small depressed="true" dark v-bind="attrs"
                v-on="on" class="mr-5">
                <v-icon x-large color="error">fab fa-linkedin</v-icon>
            </v-btn></a>
    <a href="https://github.com/lukastars" target="_blank" class="link-btn">  <v-btn large style="background-color: #252835;" fab small depressed="true" dark v-bind="attrs"
                v-on="on" class="mr-5">
                <v-icon x-large color="error">fab fa-github</v-icon>
              </v-btn></a>
      <a href="mailto:bonger2014@gmail.com" target="_blank" class="link-btn"><v-btn large style="background-color: #252835;" fab small depressed="true" dark v-bind="attrs"
                v-on="on">
                <v-icon x-large color="error">far fa-envelope</v-icon>
              </v-btn></a>
    </div>
    </v-flex>
    
  </v-container> 

  </div>
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
      selector: ['#projects', '#about', '#home'],
      selected: 'Button',
      duration: 700,
      offset: 30,
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
.contact-title {
  font-size: 48px;
  color: #ffff;
  font-family:'Tienne', serif;
  font-weight: 700;
}
.contact-p {
  font-size: 20px;
  color: #ffff;
  font-family:'Tienne', serif;
  font-weight: 400;
}
.contact-section {
  background-color: black;
}

.wave-section {
  background-image: url("../assets/wave.svg");
  background-color: #e877a6;
  background-size: 108%;
}

@media (max-width: 479px) {
  .contact-title {
    font-size: 32px;
  }
  .contact-p {
  font-size: 16px;
  }
}
</style>