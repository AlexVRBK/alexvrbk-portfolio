<template>
  <div class="flex flex-col gap-[2.5rem]">
    <!-- introduction section -->
    <div class="divCenter">
      <p
        id="landing_intro"
        ref="landingIntro"
        class="lg:text-xl text-md acrlyic w-auto text-center selector"
      ></p>
    </div>
    <section class="">
      <h1 class="text-4xl font-bold">Alexandr Vorobok</h1>
      <h3 class="text-lg">Professional Front-end developer</h3>
    </section>
    <section class="pt-2">
      <h2
        class="lg:text-2xl text-lg font-bold underline underline-offset-8 decoration-2"
      >
        Professional background
      </h2>
      <br />
      <p class="lg:text-lg text-sm text-justify leading-6">
        &nbsp;&nbsp;&nbsp;&nbsp; A professional front-end developer capable of building
        <strong>professional-looking and user-friendly websites from the ground up, and writing performance-optimized code</strong>
        that can be reused and repurposed.
      </p>
      <br />
      <p class="lg:text-lg text-sm text-justify leading-6">
        <!-- &nbsp;&nbsp;&nbsp;&nbsp; -->
        Every project I am proud of includes modern frameworks and technologies such as <strong>HTML, CSS, JavaScript and their ecosystems such as Vue.js or Nuxt. I also have experience with handy development tools like Git and Webpack.</strong> <br> <br>
        In my portfolio, you will find projects of various levels of complexity - from one-page landing pages to complex web applications with advanced interaction capabilities and built-in animations. I always try to find optimal solutions and bring maximum benefit to the project using best development practices. <br> <br>
        In addition, <strong>I am an active team player and able to communicate effectively with designers and other developers to achieve a common goal.</strong> I am always open to learning new technologies and improving my skills to bring more innovation to my work. <br> <br>
        My portfolio is an embodiment of my creativity and my skills as a frontend developer.The differences of each project are highlighted through aesthetic design, functionality and intuitive user experience. <br> <br>  
        I invite you to familiarize yourself with my projects and observe
      </p>
    </section>
    <!-- info section -->
    <!-- <section class="">
      <h2
        class="lg:text-2xl text-lg font-bold underline underline-offset-8 decoration-2"
      >
        Bio
      </h2>
      <br />
      <p class="lg:text-lg text-sm text-justify leading-6">
        &nbsp;&nbsp;&nbsp;&nbsp; Alex has a strong passion on technology and
        computers. Outside of programmimg, Aaron has a hobby of collecting and
        engage with technology. He likes to tinker with his Arch Linux Operating
        System and enjoys collecting custom keyboards.
      </p>
    </section> -->
    <!-- journey section -->
    <!-- <section class="">
      <h2
        class="lg:text-2xl text-lg font-bold underline underline-offset-8 decoration-2"
      >
        Journey
      </h2>
      <br />
      <div class="flex flex-col gap-2">
      
        <p class="lg:text-lg text-sm text-justify">
          <strong>2017:</strong>
          &nbsp; Started journey on programming as a hobby
        </p>
       
        <p class="lg:text-lg text-sm text-justify">
          <strong>2020:</strong>
          &nbsp; Enrolled for diploma of ICT with specalism in software
          engineering
        </p>
        
        <p class="lg:text-lg text-sm text-justify">
          <strong>2022:</strong>
          &nbsp; Started journey on web development
        </p>
      </div>
    </section> -->
  </div>
</template>

<script>
import TypeIt from 'typeit';
import 'animate.css';
import { ref } from 'vue';

export default {
	data() {
		return {
			display: false,
		};
	},
	setup() {
		const landingIntro = ref('');

		if (landingIntro.value !== '') {
			landingIntro.value === '';
		}
	},
	mounted() {
		new TypeIt('#landing_intro', {
			speed: 50,
			waitUntilVisible: true,
			startDelay: 2000,
			startDelete: true,
			// remove cursor when finished
			afterComplete: function (instance) {
				instance.destroy();
			},
		})
			.type('Hello! I am a Front-end developer based in Ukraine.')
			.go();
	},
};
</script>

<style>
.selector {
  background-color: var(--bg-sel);
}

.copyright {
  animation: fadeInLeft; 
  animation-duration: 1s; 
  animation-delay: 3s;
}

/* @keyframes copyright {
  0% {
    opacity: 0;
  }
  100% {
    opacity: 1;
    visibility: visible;
  }
} */
</style>
