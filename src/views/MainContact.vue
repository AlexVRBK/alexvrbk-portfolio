<template>
  <div>
    <section class="">
      <h2
        class="lg:text-2xl text-lg font-bold underline underline-offset-8 decoration-2"
      >
        Get in touch
      </h2>
      <br />
      <!-- <p class="lg:text-lg text-sm text-justify leading-6">
        &nbsp;&nbsp;&nbsp;&nbsp; Have an idea you want it to become a reality? I
        can make it happen for you! Don't feel hesitated to contact me, I will
        be responding to your messages as soon as possible.
      </p> -->
    </section>
    <section
      class="divCenter pt-5 8xl:ml-[-70rem] 7xl:ml-[-55rem] 6xl:ml-[-20rem] 5xl:ml-[-10rem] 4xl:ml-[-5rem] 3xl:ml-[-2rem] xl:mr-[40rem] lg:mr-[27rem] md:mr-[15rem] sm:ml-[0rem] ml-[3rem] flex flex-col w-full"
    >
      <div id="Contact_ThreeContainer" class="-mt-10 pl-20 hidden"></div>
    </section>
    <section class="pt-5">
      <p class="lg:text-lg text-sm text-justify leading-6">
        You can reach me by emailing me at
        <strong>vvvorobok@gmail.com</strong>. I will be able to reply to your
        mail.
      </p>
    </section>
    <br />
    <section class="">
      <p class="lg:text-lg text-sm text-justify leading-6">
        You can visit my
        <strong class="underline"
          ><router-link to="/work">portfolio</router-link></strong
        >
        to view my works. Alternatively, you can visit my
        <strong class="underline"
          ><a href="https://github.com/AlexVRBK">Github Profile</a></strong
        >
        to view my projects posted on Github
        <br><br>
         You can also go to my 
        <strong class="underline"
          ><a href="https://www.linkedin.com/in/alexvorobok/">LinkedIn profile</a></strong
        >
      </p>
    </section>
  </div>
</template>

<script>
import { ref } from 'vue';

export default {
	setup() {
		
	}
};
</script>

<style scoped>
  hr {
    border-color: var(--text);
  }

  input {
    background-color: var(--bg-sel);
    border-color: var(--text-highlight);
  }

  input:focus {
    border-color: var(--text-highlight-2);
  }

  textarea {
    background-color: var(--bg-sel);
    border-color: var(--text-highlight);
  }

  textarea:focus {
    border-color: var(--text-highlight-2);
  }

  button {
    background-color: var(--bg-sel);
  }

  .success {
    color: var(--text-highlight);
  }
</style>
