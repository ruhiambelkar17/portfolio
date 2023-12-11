<script>
import  Email  from "@/assets/smtp/smtp.js";

export default {
  data() {
    return {
      name: "",
      email: "",
      message: "",
      subject:"",
    };
  },
  methods: {
    sendMail() {
        console.log("email:",this.email,"Name:",this.name,"subj:",this.subject,"msg:",this.message);
      Email.send({
        SecureToken: "db03cdbd-940e-4cd9-ab60-8b5cb816888e",
        To: "ruhiambelkar7@gmail.com",
        From: this.email,
        name:this.name,
        Subject:this.subject,
        Body: this.message,
      }).then((message) => alert(message));
    },
  },
};
</script>

<template>
  <div class="row my-5">
    <div class="col-md-6 offset-md-3">
      <div id="contact-heading">
        <h1 class="display-1 text-center">Contact Me</h1>
      </div>
      <form class="border rounded p-5 shadow">
        <div class="mb-3">
          <label for="name" class="form-label">Name</label>
          <input type="text" id="name" class="form-control" v-model="name" />
        </div>
        <div class="mb-3">
          <label for="subject" class="form-label">Subject</label>
          <input type="text" id="subject" class="form-control" v-model="subject" />
        </div>
        <div class="mb-3">
          <label for="email" class="form-label">Email</label>
          <input type="email" id="email" class="form-control" v-model="email" />
        </div>
        <div class="mb-3">
          <label for="name" class="form-label">Messase</label>
          <textarea rows="4" id="name" class="form-control" v-model="message" />
        </div>
        <div class="d-flex justify-content-center mt-4">
          <input class="btn btn-primary" type="button" value="Submit" @click="sendMail()" />
        </div>
      </form>
    </div>
  </div>
</template>
<style scoped>
#contact-heading {
  background: -webkit-linear-gradient(141deg, rgba(2,0,36,1) 0%, rgba(4,46,49,1) 25%, rgba(0,212,255,1) 100%);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}


form {
  color: rgb(4, 46, 49);
  background-color: rgb(148, 205, 209) !important ;
}

.btn {
  background-color: rgb(4, 46, 49);
  border-color: rgb(4, 46, 49);
  width: 200px;
}
</style>
