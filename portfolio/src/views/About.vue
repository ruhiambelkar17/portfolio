<script></script>

<template>
  <div class="row my-5 bg-light">
    <div class="col-md-12">
      <div
        id="about-heading"
        class=""
      >
        <!-- <img class="" id="about-img" src="../assets/images/women_avatar.png" /> -->
        <h1 class="display-1">About</h1>
        <p id="about-line"></p>
      </div>
      <div id="about-content" class="row">
        <div class="col-md-4 offset-md-1">
            <h1>I'm a Front End Developer!!</h1>
          <p>
            I'm a Frontend Web Developer building the Front-end of Websites and
            Web Applications that leads to the success of the overall product.
            Check out some of my work in the Projects section. I also like
            sharing content related to the stuff that I have learned over the
            years in Web Development so it can help other people of the Dev
            Community. Feel free to Connect or Follow me on my Linkedin where I
            post useful content related to Web Development and Programming I'm
            open to Job opportunities where I can contribute, learn and grow. If
            you have a good opportunity that matches my skills and experience
            then don't hesitate to contact me.
          </p>
        </div>
        <div class="col-md-4 offset-md-1">
            <h1>My skills</h1>
            <span class="badge " id="about-badge">Vue JS</span>
            <span class="badge" id="about-badge">React</span>
            <span class="badge" id="about-badge">Typescript</span>
            <span class="badge" id="about-badge">JavaScript</span>
            <span class="badge" id="about-badge">Node Js</span>
            <span class="badge" id="about-badge">Rest API</span>
            <span class="badge" id="about-badge">HTML</span>
            <span class="badge" id="about-badge">CSS</span>
            <span class="badge" id="about-badge">SQL</span>
        </div>
      </div>
    </div>
  </div>
</template>

<style>
#about-img {
  height: 300px;
  width: 300px;
  background-color: bisque;
  border: 5px black solid;
  border-radius: 50%;
}

#about-heading {
  /* background-color: rgb(4, 46, 49); */
  color: rgb(4, 46, 49);
  height: 100px;
  width: 100%;
}

#about-line {
    height: 5px;
    width: 100px;
    background-color:rgb(148, 205, 209) ;
    margin-left: 47%;
}

#about-content {
  margin-top: 100px;
  color: rgb(4, 46, 49);
}
#about-badge {
    height: 40px;
    width: auto;
    background-color:rgb(148, 205, 209) ;
    font-size: 20px;
    margin: 10px;
}
</style>
