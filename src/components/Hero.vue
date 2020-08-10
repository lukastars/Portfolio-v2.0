<template>
<div id="home">
  <v-container class="d-flex justify-center">  
      <v-flex col-lg-7 col-md-9 col-sm-12 col-xs-12>
         <div class="d-flex justify-center pics">
          <img src="@/assets/coding.svg" alt="" class="tech-logo col-lg-2" >
          <img src="@/assets/css.svg" alt="" class="tech-logo  col-lg-2">
          <img src="@/assets/statistics.svg" alt="" class="tech-logo col-lg-2">
          <img src="@/assets/api.svg" alt="" class="tech-logo col-lg-2">
          <img src="@/assets/student.svg" alt="" class="tech-logo col-lg-2">
        </div> 
      <div class="header">
        <div class="header-background"></div>
        <div><h1 style="text-shadow: 2px 2px 4px #000000;" class="hero-title d-flex justify-center text-center">Hi There</h1></div>
      </div>
      
      <p class="hero-text text-center">My Name is Ali and I'm a Front-End Web Developer. I Love Turning Exciting Ideas Into Beautiful Modern and Responsive Websites & Web Applications.</p>
      <div class="d-flex justify-center mt-12">
     <a href="#projects" class="link-btn"><v-btn rounded="true" large="true" @click="$vuetify.goTo(target[0], options)">
          <span class="projects-btn">Projects</span>
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
.tech-logo {
  max-width: 90px;
  animation: float 6s ease-in-out infinite;
}

.hero-title {
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

.header-background {
  background-image: url("../assets/drawings.svg");
  background-position: 0% 0%;
  background-size: 100%;
  background-repeat: no-repeat;
  position: absolute;
  height: 100%;
  width: 100%;
  z-index: 0;
  animation: float 7s ease-in-out infinite;
}

.hero-text {
  font-size: 22px;
  color: #ffff;
  font-family:'Tienne', serif;
  font-weight: 400;
}
.projects-btn {
  font-family: 'Alegreya Sans', sans-serif;
  color: #252835;
  font-weight: 900;
}

@media (max-width: 479px) {
  .pics {
    max-width: 100%;
  }
}
@media (max-width: 991px) {
  .hero-title {
  font-size: 100px;
  }
  

}
@media (max-width: 479px) {
  .hero-title {
  font-size: 78px;
  }
  .hero-text {
    font-size: 17px;
  }
  .header-background {
    background-size: 100%;
  }
  .tech-logo {
    max-width: 64px;
  }
}

@keyframes float {
	0% {
		transform: translatey(0px);
	}
	50% {
		transform: translatey(-20px);
	}
	100% {
		transform: translatey(0px);
	}
}
</style>
