<script>
export default {};
</script>

<template>
  <div class="row mt-5">
    <div class="col-md-10 offset-md-1 projects-container shadow">
      <div class="d-inline-flex">
        <img src="../assets/images/work.png" width="150px" height="150px" />
        <h1 class="my-5 pg-heading">Clients I worked with</h1>
      </div>
      
      <div class="row">
        <div class="col-md-4 mt-5">
          <div class="card">
            <img
              src="../assets/images/Lumen_Technologies_Logo.png"
              class="mx-auto d-block"
              alt="Lumen"
              height="70px"
              width="100px"
            />

            <div class="card-body">
              <h5 class="card-title">Vue JS End Developer</h5>
              <p class="card-text">
                Developed Telecom based application from initial design using
                HTML,CHI Design System(CSS Framework by Lumen) and Vue JS
                components using Composition API and Typescript.
              </p>
              <span class="badge rounded-pill   ">Vue JS</span>
              <span class="badge rounded-pill   ">Typescript</span>
              <span class="badge rounded-pill  ">HTML</span>
              <span class="badge rounded-pill  ">CSS</span>
              <span class="badge rounded-pill  ">REST Api</span>
              <!-- <a href="#" class="btn btn-primary">Go somewhere</a> -->
              <!-- <ul>
                      <li>Developed Telecom based application from initial design using HTML,CHI Design System(CSS Framework by Lumen) and Vue JS components using Composition API and Typescript. </li>
                      <li>Utilized Vue.JS libraries like Vue-Router for navigation between different components, Vee-Validate for form validation, Vuex for State management and Axios library for API integration.</li>
                      <li>Implemented Vue.JS concepts like props, emits,watch,computed properties, slots, lifecycle hooks, axios, vuex-store.,etc.</li>
                      <li>Closely worked with Business Analyst to understand business requirements to ensure that right set of UI modules been built. </li>
                      <li>Collaborated with the back-end team and successfully integrated RESTful APIs. </li>
                      <li>Collaborated with QA team to get insights on key areas of improvement. </li>
                      <li>Wrote e2e test cases with Cypress and Unit test cases with Chai and Mocha to ensure 100% bug free Application. </li>
                      <li>Wrote clean, maintainable, and efficient code in line with the latest web standards. </li>
                      <li>Worked in Agile environment, kept track of user stories in Jira, participated in Sprint planning.</li>
                      <li>Managed deployments with GitHub actions and designed workflow with Sonarqube, Test flow, Code Security and Deployment triggers.</li>
                      <li>Mentored junior team, enabling them to achieve professional growth and personal goals.</li>
                    </ul> -->
            </div>
          </div>
        </div>
        <div class="col-md-4 mt-5">
          <div class="card">
            <img
              src="../assets/images/Telenor-logo.png"
              alt="Telenor"
              class="mx-auto d-block"
              height="70px"
              width="100px"
            />

            <div class="card-body">
              <h5 class="card-title">Front End Developer</h5>
              <p class="card-text">
                Designed and Developed Telecom based application from initial
                design using Figma, HTML, Bootstrap and Vue JS components using
                JavaScript.
              </p>
              <span class="badge rounded-pill  ">Vue JS</span>
              <span class="badge rounded-pill  ">JavaScript</span>
              <span class="badge rounded-pill  ">HTML</span>
              <span class="badge rounded-pill  ">Bootstrap</span>
              <span class="badge rounded-pill  ">REST Api</span>
            </div>
          </div>
        </div>
        <div class="col-md-4 mt-5">
          <div class="card">
            <img
              src="../assets/images/Caterpillar-Logo.png"
              class="mx-auto d-block"
              alt="caterpillar"
              height="70px"
              width="100px"
            />

            <div class="card-body">
              <h5 class="card-title">Front End Developer</h5>
              <p class="card-text">
                Assisted in building user friendly internal web application to manage Database to meet client requirements. 
              </p>
              <span class="badge rounded-pill  ">Vue JS</span>
              <span class="badge rounded-pill  ">HTML</span>
              <span class="badge rounded-pill  ">CSS</span>
              <span class="badge rounded-pill  ">MySQL</span>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.pg-heading {
  
  background: -webkit-linear-gradient(141deg, rgba(2,0,36,1) 0%, rgba(4,46,49,1) 25%, rgba(0,212,255,1) 100%);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}
.projects-container {
  background-color: white;
  height: 100vh;
  border-radius: 50px;
  color: rgb(4, 46, 49);
}

p {
  font-size: small;
}

.badge {
  background-color:rgb(148, 205, 209) !important ;
  margin-right: 10px;
  color: white;
}
</style>
