<template>
  <Navbar />
  <Header />
  <Services />
  <About />

  <div class="bg-green-50 py-5 page-section">
    <div class="container">
      <div class="text-center wow fadeInUp">
        <div class="text-2xl mb-3">Personality as Developer</div>
        <h3 class="title-section">
          <span>"Slow and Steady</span>
          Win The Rase"
        </h3>
        <div class="divider mx-auto"></div>
      </div>

      <div
        class="flex flex-col lg:flex-row items-center justify-evenly space-x-3 h-full text-left py-5">
        <div
          class="bg-white rounded-xl drop-shadow-md mt-3 col-lg-4 ml-2 py-1 px-5 h-96 hover:-mt-3 cursor-default hover:shadow-lg hover:shadow-green-100">
          <lord-icon
            src="https://cdn.lordicon.com/dfxesbyu.json"
            trigger="hover"
            style="width: 150px; height: 150px"
            class="hidden lg:flex"></lord-icon>

          <div class="text-2xl font-semibold text-green-800 mt-4 pl-1">
            Quick Learning
          </div>
          <p class="text-left text-base lg:text-sm leading-relaxed">
            Best software developers are often fantastic self-learners.The ideal
            skill any person can have is understanding how to learn, and ideal
            developers have acquired the skill of self-learning.
          </p>
        </div>

        <div
          class="bg-white rounded-xl mt-3 drop-shadow-md col-lg-4 ml-2 py-1 px-5 h-96 hover:-mt-3 cursor-default hover:shadow-lg hover:shadow-green-100">
          <lord-icon
            src="https://cdn.lordicon.com/xqgancly.json"
            trigger="hover"
            style="width: 150px; height: 150px"
            class="hidden lg:flex"></lord-icon>

          <div class="text-2xl font-semibold text-green-800 mt-4 pl-1">
            Problem Solving
          </div>
          <p class="text-left text-base lg:text-sm leading-relaxed">
            Problem-solving is a one of the most important part of the work.
            Problem-solving also has to do with utilizing creativity and logical
            thought processes to identify problems and resolve them with
            software.
          </p>
        </div>

        <div
          class="bg-white rounded-xl drop-shadow-md mt-3 col-lg-4 ml-2 py-1 px-5 h-96 hover:-mt-3 cursor-default hover:shadow-lg hover:shadow-green-100">
          <lord-icon
            src="https://cdn.lordicon.com/hursldrn.json"
            trigger="morph"
            style="width: 150px; height: 150px"
            class="hidden lg:flex"></lord-icon>

          <div class="text-2xl font-semibold text-green-800 mt-4 pl-1">
            Honesty
          </div>
          <p class="text-left text-base lg:text-sm leading-relaxed">
            Software developers need to learn to admit their mistakes. Of
            course, making a mistake occurs to all of us. The most important
            thing to do is to make an effort to learn from them and try to avoid
            them later in life.
          </p>
        </div>
      </div>
    </div>
  </div>

  <Blog :blog="blog" />
  <Footer />
</template>

<script>
import Navbar from "./Navbar.vue";
import Header from "./Header.vue";
import Services from "./Services.vue";
import About from "./About.vue";
import Projects from "./Projects.vue";
import Contact from "./Contact.vue";
import Blog from "./Blog.vue";
import Footer from "./Footer.vue";

export default {
  mounted() {
 
  (function(d, m){
      var kommunicateSettings = 
          {"appId":"24577ce21c5e5fda55ffe75941e94bed9","popupWidget":true,"automaticChatOpenOnNavigation":true};
      var s = document.createElement("script"); s.type = "text/javascript"; s.async = true;
      s.src = "https://widget.kommunicate.io/v2/kommunicate.app";
      var h = document.getElementsByTagName("head")[0]; h.appendChild(s);
      window.kommunicate = m; m._globals = kommunicateSettings;
  })(document, window.kommunicate || {});
  /* NOTE : Use web server to view HTML files as real-time update will not work if you directly open the HTML file in the browser. */

},
  name: "Home",
  data() {
    return {};
  },

  props: {
    blog: Array,
  },

  components: {
    Navbar,
    Header,
    Services,
    About,
    Projects,
    Contact,
    Blog,
    Footer,
  },
};
</script>

<style></style>
