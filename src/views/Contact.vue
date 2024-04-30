<script>
//import Email from "@/assets/smtp/smtp.js";
import emailjs from "emailjs-com";

export default {
  data() {
    return {
      name: "",
      email: "",
      message: "",
    };
  },
  methods: {
    sendMail() {
      console.log(
        "email:",
        this.email,
        "Name:",
        this.name,
        "subj:",
        "msg:",
        this.message
      );
     
      // emailjs.sendForm(
      //   "service_qa87qk5",
      //   "template_jgabish",
        
      //   // {
      //   //   message: this.message,
      //   //   name: this.name,
      //   //   mail: this.mail,
      //   // },
      //   this.$refs.form,
      //   // {
      //   //   publicKey: 'YOUR_PUBLIC_KEY',
      //   // }
        
      // );

      emailjs.sendForm('service_qa87qk5', 'template_jgabish', this.$refs.form,"wYsUv-8XAeSmUfOs5").then(
  (response) => {
    console.log('SUCCESS!', response.status, response.text);
  },
  (error) => {
    console.log('FAILED...', error);
  },
);
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
      <form class="border rounded p-5 shadow" ref="form" @submit.prevent="sendMail">
        <div class="mb-3">
          <label for="name" class="form-label">Name</label>
          <input type="text" id="name" class="form-control" v-model="name" name="name" />
        </div>

        <div class="mb-3">
          <label for="email" class="form-label">Email</label>
          <input type="email" id="email" class="form-control" v-model="email" name="email" />
        </div>
        <div class="mb-3">
          <label for="message" class="form-label">Messase</label>
          <textarea rows="4" id="message" class="form-control" v-model="message" name="message" />
        </div>
        <div class="d-flex justify-content-center mt-4">
          <input type="submit" class="btn btn-primary" value="Send">
          
        </div>
      </form>
    </div>
  </div>
</template>
<style scoped>
#contact-heading {
  background: -webkit-linear-gradient(
    141deg,
    rgba(2, 0, 36, 1) 0%,
    rgba(4, 46, 49, 1) 25%,
    rgba(0, 212, 255, 1) 100%
  );
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
