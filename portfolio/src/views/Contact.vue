<script>

export default {
    data(){
        return {
            name:"",
            email:"",
            message:""
        }
    }
}
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
            <input type="text" id="name" class="form-control" v-model="name"/>
        </div>
        <div class="mb-3">
            <label for="name" class="form-label">Email</label>
            <input type="text" id="name" class="form-control" v-mode="email"/>
        </div>
        <div class="mb-3">
            <label for="name" class="form-label">Messase</label>
            <textarea rows="4" id="name" class="form-control" v-mode="message" />
        </div>
        <div class="d-flex justify-content-center mt-4">
            <input class="btn btn-primary" type="submit" value="Submit">
        </div>
        
      </form>
    </div>
  </div>
</template>
<style scoped>
#contact-heading {
  color: rgb(4, 46, 49);
  
}

form {
    color: rgb(4, 46, 49);
    background-color:rgb(148, 205, 209) !important ;
}

.btn {
    background-color:rgb(4, 46, 49) ;
    border-color: rgb(4, 46, 49);
    width: 200px;
}
</style>
