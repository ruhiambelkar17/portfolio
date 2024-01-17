<script>
export default{
  data(){
    return {
      scrollToPage:""
    }
  },
  methods: {
    scrollTo(dest) {
      this.scrollToPage=dest,
      this.$emit("scrollTo", this.scrollToPage);
    },

  },
}
</script>

<template>
    <div>
        <nav class="navbar navbar-expand-lg bg-body-tertiary shadow ">
        <div class="container-fluid">
          <a class="navbar-brand ms-5 text-style" href="#"
            >Ruhi Ramakant Ambelkar</a
          >
          <button
            class="navbar-toggler"
            type="button"
            data-bs-toggle="collapse"
            data-bs-target="#navbarSupportedContent"
            aria-controls="navbarSupportedContent"
            aria-expanded="false"
            aria-label="Toggle navigation"
          >
            <span class="navbar-toggler-icon"></span>
          </button>

          <div class="collapse navbar-collapse justify-content-end " id="navbarSupportedContent">
            <ul class="navbar-nav ms-5">
            <li class="nav-item p-3">
              <a class="nav-link" href="#" >Home</a>
            </li>
            <li class="nav-item p-3">
              <a class="nav-link" href="#" @click="scrollTo('projects')">Projects</a>
            </li>
            <li class="nav-item p-3">
              <a class="nav-link" href="#" @click="scrollTo('about-me')">About</a>
            </li>
            <li class="nav-item p-3">
              <a class="nav-link" href="#" @click="scrollTo('contact-me')">Contact</a>
            </li>
          </ul>
          </div>
        </div>
      </nav>
    </div>
</template>