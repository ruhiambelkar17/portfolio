<script>
import Nav from "../components/Nav.vue";
import Footer from "../components/Footer.vue";
import Projects from "./Projects.vue";
import About from "./About.vue";
import Contact from "./Contact.vue";

export default {
  components: {
    Nav,
    Projects,
    About,
    Footer,
    Contact,
  },
  data() {
    return {
      scrollToSection: "",
      isArr: true,
      arr: [1, 2, 3, 4, 5],
    };
  },
  methods: {
    scrollToView(scrollToPage) {
      console.log("scrollToPage", scrollToPage);
      this.scrollToSection = scrollToPage;
      const element = document.getElementById(this.scrollToSection);
      element.scrollIntoView({ behavior: "smooth" });
    },
    // scrollToSection() {
    //   const element = document.getElementById(thos.scrollToPage);
    //   element.scrollIntoView({ behavior: 'smooth' });
    // },
  },
};
</script>

<template>
  <div>
    <Nav @scrollTo="scrollToView" />

    <div class="container-1">
      <div class="d-flex justify-content-between">
        <img
          src="../assets/images/vue.png"
          width="100px"
          height="100px"
          class="icon-left-top"
        />
        <img
          src="../assets/images/react.png"
          width="100px"
          height="100px"
          class="icon-right-top"
        />
      </div>
      <div class="d-flex justify-content-center mt-2">
        <img
          class="shadow"
          id="avatar"
          src="../assets/images/women_avatar.png"
        />
      </div>
      <div class="d-flex justify-content-between">
        <img
          src="../assets/images/js.png"
          width="100px"
          height="100px"
          class="icon-left-bottom"
        />
        <img
          src="../assets/images/api.png"
          width="100px"
          height="100px"
          class="icon-right-bottom"
        />
      </div>
      <h1 class="text-center text-style pg-heading">
        Front-End Web Developer {{ scrollToSection }}
      </h1>
      <div class="row text-center text-style">
        <div class="col-md-6 offset-md-3">
          <p>
            I am an Experienced Front End Web developer with 5 years of
            experience in creating Mobile responsive web applications.
          </p>
          <div class="d-flex justify-content-center">
            <button
              class="btn border button-style"
              @click="scrollToView('contact-me')"
            >
              Contact Me
            </button>
          </div>
        </div>
      </div>
    </div>
    <div class="d-flex justify-content-center mt-5 mb-0">
      <img width="700" src="../assets/images/web-design-1.png" />
    </div>
    <div class="container-2">
      <div class="text-center pt-5">
        <h2>Hello, I am Ruhi! Nice to meet you!</h2>
        <div class="row text-center">
          <div class="col-md-6 offset-md-3">
            <p>
              I am a passionate Front End Developer with 5 years of experience
              in designing, developing, testing and maintaining mobile
              responsive web applications. Adept in contributing to highly
              collaborative work environment, finding solutions and determining
              customer satisfaction.
            </p>
          </div>
        </div>
        <Projects id="projects" />
      </div>
      <About id="about-me" />
      <Contact id="contact-me" />
      <Footer />
    </div>
  </div>
</template>

<style scoped>
.pg-heading {
  background: -webkit-linear-gradient(
    141deg,
    rgba(2, 0, 36, 1) 0%,
    rgba(4, 46, 49, 1) 25%,
    rgba(0, 212, 255, 1) 100%
  );
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}

#avatar {
  height: 250px;
  width: 250px;
  background-color: bisque;
  border: 5px black solid;
  border-radius: 50%;
}

@keyframes leftTop {
  0% {
    left: 0px;
    top: 0px;
  }
  100% {
    left: 450px;
    top: 100px;
  }
}

@keyframes rightTop {
  0% {
    right: 0px;
    top: 0px;
  }
  100% {
    right: 450px;
    top: 100px;
  }
}

@keyframes leftBottom {
  0% {
    left: 0px;
    bottom: 0px;
  }
  100% {
    left: 350px;
    bottom: 100px;
  }
}

@keyframes rightBottom {
  0% {
    right: 0px;
    bottom: 0px;
  }
  100% {
    right: 350px;
    bottom: 100px;
  }
}
.icon-left-top {
  position: relative;
  animation-name: leftTop;
  animation-duration: 4s;
  animation-fill-mode: forwards;
}

.icon-right-top {
  position: relative;
  animation-name: rightTop;
  animation-duration: 4s;
  animation-fill-mode: forwards;
}
.icon-left-bottom {
  position: relative;
  animation-name: leftBottom;
  animation-duration: 4s;
  animation-fill-mode: forwards;
}

.icon-right-bottom {
  position: relative;
  animation-name: rightBottom;
  animation-duration: 4s;
  animation-fill-mode: forwards;
}

.button-style {
  background: rgb(2, 0, 36);
  background: linear-gradient(
    -130deg,
    rgba(2, 0, 36, 1) 0%,
    rgba(4, 46, 49, 1) 45%,
    rgba(0, 212, 255, 1) 100%
  );
  color: white;
}

.container-2 {
  background-color: rgb(4, 46, 49);
  height: 50vh;
  border-top-left-radius: 50px;
  border-top-right-radius: 50px;
  color: white !important;
}
</style>
